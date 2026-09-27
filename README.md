# 🫙 Cofrinho
 
App para criar metas e registrar cada valor guardado.
 
- Cada meta vira um pote que enche conforme você guarda dinheiro
- Registro de depósitos e retiradas com data, origem e anotação
- Cálculo de quanto guardar por mês/semana para bater a meta no prazo
- Backup e restauração em arquivo `.json`
## Dados e segurança
Login com e-mail e senha (Supabase Auth). Metas e registros ficam no Supabase,
esquema `cofrinho`, com Row Level Security: cada usuário só lê e altera os próprios dados.
A chave no `index.html` é a chave pública (publishable) — pode ficar no código.