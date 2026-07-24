# GamaERP — Vigia externo

Monitor independente (GitHub Actions) que testa a cada ~15 min se o **GamaERP** (Vercel) e o banco (**Neon**) estao no ar, chamando um endpoint publico que toca o banco.

Se falhar 3x seguidas, o job falha e o **GitHub avisa o dono por e-mail** — inclusive quando a causa e pagamento/limite (o vigia roda fora da Vercel e do Neon, entao nao cai junto).
