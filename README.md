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
- `INDEX.md` - полный список всех спецификаций со статусами
- `specs/README.md` - процесс создания и утверждения спецификаций

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
