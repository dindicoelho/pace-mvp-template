# Estratégia de Versionamento de API

## 🎯 Para MVP: Keep It Simple

### Estratégia Escolhida: URL Path Versioning
/api/v1/users
/api/v1/products
/api/v1/orders

## 🔨 Implementação Prática

### 1. Criar rota versionada:

```typescript
// src/app/api/v1/users/route.ts
export async function GET(request: Request) {
  return Response.json({
    version: "1.0",
    data: users
  })
}

2. Quando criar v2?
NÃO crie v2 para:

Adicionar campos novos (retrocompatível)
Corrigir bugs
Melhorar performance

CRIE v2 quando:

Remover campos obrigatórios
Mudar formato de resposta
Alterar lógica core

3. Deprecação (quando chegar lá):
typescript// src/app/api/v1/users/route.ts
export async function GET(request: Request) {
  return Response.json({
    version: "1.0",
    deprecated: true,
    message: "Use /api/v2/users",
    sunset: "2025-12-31",
    data: users
  })
}