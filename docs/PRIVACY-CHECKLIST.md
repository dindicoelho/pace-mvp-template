# Checklist de Privacidade - LGPD/GDPR Básico

## ⚠️ MVP Mínimo Legal

### Coleta de Dados
- [ ] **Coletando apenas o essencial?**
  - Email, nome, senha
  - Não pedir CPF, telefone, endereço se não precisa

- [ ] **Aviso de coleta claro?**
  - "Vamos usar seu email para login e contato"
  - Não esconder em letras miúdas

### Consentimento
- [ ] **Checkbox de aceite nos termos?**
  - "Li e aceito os termos de uso"
  - NÃO pode vir marcado por padrão

- [ ] **Link para política de privacidade?**
  - Pode ser simples, mas precisa existir
  - Exemplo: `/privacy-policy`

### Segurança Básica
- [ ] **Senhas hasheadas?**
  - NUNCA salvar senha em texto puro
  - Use bcrypt ou função do Supabase

- [ ] **HTTPS em produção?**
  - Vercel faz isso automaticamente ✅
  
- [ ] **Dados sensíveis no .env?**
  - API keys nunca no código
  - Use variáveis de ambiente

### Direitos do Usuário
- [ ] **Usuário pode deletar conta?**
  - Botão "Deletar minha conta"
  - Deleta TODOS os dados

- [ ] **Usuário pode ver seus dados?**
  - Página de perfil com infos
  - "Meus dados" mostrando o que tem salvo

- [ ] **Usuário pode corrigir dados?**
  - Editar perfil funcionando

## 📝 Texto Mínimo de Política de Privacidade

Política de Privacidade
Que dados coletamos?

Email e nome para criar sua conta
Dados que você criar no app (tarefas, notas, etc)

Como usamos?

Para fazer login
Para salvar suas informações
Para entrar em contato se necessário

Compartilhamos com alguém?

Não vendemos seus dados
Só compartilhamos se a lei exigir

Como protegemos?

Senhas criptografadas
Conexão segura (HTTPS)
Servidores seguros (Vercel/Supabase)

Seus direitos

Ver seus dados: página de perfil
Corrigir dados: editar perfil
Deletar tudo: deletar conta

Contato

Email: seu-email@exemplo.com

Última atualização: [DATA]

## ✅ Para estar OK no MVP:
1. Aviso que coleta dados
2. Botão deletar conta
3. Política de privacidade (mesmo simples)
4. Senhas hasheadas
5. HTTPS (automático no Vercel)