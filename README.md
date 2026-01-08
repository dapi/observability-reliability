# Site Reliability Specifications (SRS)

Коллекция практических руководств по построению надежных и наблюдаемых приложений.

## Описание

Репозиторий содержит практические руководства (спецификации) по построению надежных и наблюдаемых приложений, основанные на лучших практиках Site Reliability Engineering.

**Основные категории:**

- **Надежность**: Circuit Breaker, Retry, Graceful Shutdown, Jobs Management, Idempotency, Rate Limiting
- **Наблюдаемость**: Logging, Error Tracking, Liveness Probes, Versioning
- **Масштабируемость**: Scaling, Load Shedding, Load Balancing, Deadlines
- **DevOps практики**: Configuration, Environment Variables, Stand-Independent Images

## Структура репозитория

- `specs/` - директория со всеми спецификациями
- `specs/README.md` - процесс создания и утверждения спецификаций

## Каталог спецификаций

### Надежность (Reliability)

| Спецификация | Название | Статус |
|-------------|----------|--------|
| [SRS-001](specs/SRS-001%20Jobs%20Management.md) | Jobs Management | ✅ |
| [SRS-002](specs/SRS-002%20Stateless%20Services.md) | Stateless Services | ✅ |
| SRS-003 | Scaling and State | ✅ |
| SRS-015 | Blocking Timeouts | ✅ |
| SRS-010 | Liveness Probes | ✅ |
| SRS-014 | Graceful Shutdown | ✅ |
| SRS-016 | Request Idempotency | ✅ |
| [SRS-013](specs/SRS-013%20Load%20Shedding.md) | Load Shedding | ✅ |
| [SRS-025](specs/SRS-025%20Bulkhead%20Pattern.md) | Bulkhead Pattern | ✅ |
| SRS-018 | Distributed Caching | ✅ |
| [SRS-020](specs/SRS-020%20Retryier.md) | Retryier | ✅ |
| [SRS-022](specs/SRS-022%20Fallback.md) | Fallback | ✅ |
| [SRS-023](specs/SRS-023%20Load%20Balancing%20Patterns.md) | Load Balancing Patterns | ✅ |
| [SRS-024](specs/SRS-024%20Auto-scaling.md) | Auto-scaling | ✅ |
| SRS-027 | Rate Limiting | ❌ Планируется |
| [SRS-028](specs/SRS-028%20Database%20Connection%20Pooling.md) | Database Connection Pooling | ✅ |

### Безопасность (Security)

| Спецификация | Название | Статус |
|-------------|----------|--------|
| [SRS-040](specs/SRS-040%20Service%20Authentication.md) | Service Authentication | ✅ |
| [SRS-041](specs/SRS-041%20Authorization%20Pattern.md) | Authorization Pattern | ✅ |

### Наблюдаемость (Observability)

| Спецификация | Название | Статус |
|-------------|----------|--------|
| SRS-012 | Circuit Breaker | ✅ |
| SRS-008 | Logging (Журналирование) | ✅ |
| SRS-005 | Application Versioning | ✅ |
| SRS-007 | Expose Application Version | ✅ |
| SRS-006 | Metrics Collection | ✅ |
| [SRS-011](specs/SRS-011%20Distributed%20Tracing.md) | Distributed Tracing | ✅ |
| SRS-009 | Error Tracking | ✅ |
| SRS-004 | Environment Variables Usage | ✅ |
| SRS-019 | Stand-Independent Images | ✅ |
| SRS-021 | Liveness probes over command | ✅ |
| [SRS-026](specs/SRS-026%20Alerting%20Rules.md) | Alerting Rules | ✅ |

### Статус реализации

- **Всего спецификаций в реестре**: 37
- **Найдено в репозитории**: 26 (70%)
- **Отсутствует**: 11 (30%)

## Как использовать

Каждая спецификация имеет нумерацию вида `SRS-XXX`, где XXX - порядковый номер. Каждая спецификация содержит конкретные рекомендации и best practices, которые можно внедрять в ваши сервисы независимо.

Статус спецификаций:
- `DRAFT` - находится в разработке
- `PROPOSED` - предложена к применению
- `APPROVED` - одобрена и рекомендуется к использованию
- `DEPRECATED` - не рекомендуется к применению

## Внесение вклада

См. спецификацию [specs/README.md](specs/README.md) для информации о процессе создания новых спецификаций.

---

*Site Reliability Specifications (SRS) - практические руководства для построения production-ready систем*
