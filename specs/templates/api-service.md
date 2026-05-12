# Spec Template: API Service

## Service: [NOMBRE]
## Date: [FECHA]
## Framework: [Express|FastAPI|Fastify]

## Description
[Descripcion del servicio]

## Endpoints
| Method | Path | Description | Auth |
|--------|------|-------------|------|
| GET | /api/[resource] | List | No |
| POST | /api/[resource] | Create | Yes |
| GET | /api/[resource]/:id | Get by ID | No |
| PUT | /api/[resource]/:id | Update | Yes |
| DELETE | /api/[resource]/:id | Delete | Yes |

## Data Models
```typescript
interface [Model] {
  id: string;
  // fields
}
```

## Auth
- [JWT|OAuth|API Key]

## Acceptance Criteria
- [ ] [Criterio 1]
- [ ] [Criterio 2]
