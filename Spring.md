JPA Entity
Spring Data
Spring Repository
- Это несколько интерфейсов которые используют JPA Entity для взаимодействия с ней. Например:
  - CrudRepository<T, ID extends Serializable> - обеспечивает основные операции по поиску, сохранения, удалению данных (CRUD операции)
