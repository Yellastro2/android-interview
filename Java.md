## Multitreading
  - Mutex - MUTual EXclusion - сущность имеющаяся у каждого обьекта и закрывающая доступ к обьекту для других потоков, если один поток уже его использует. С ним работает только JVM, программно не управляется.
  - Monitor - сущность которая связывает боки помеченые synchronized и логику работы Mutex
  - Semaphore - Обьект с помощью которого можно управлять доступом к синхронному блоку нескольких потоков. Semaphore(int permits, boolean fair) задает число потоков и порядок получения ими доступа. Внутри потока acquire() и release() просят у семафора доступ, и говорят о завершении работы

  - Atomic : типы способные работать с несколькими потоками без блока synchronized. Реализуют механизм Compare-And-Swap, означаущий, что поток поменяет значение переменной только если результат будет соотв. ожидаемому
  - volatile : модификатор переменной, означающий что ее могут менять разные потоки одновременно, и каждый увидит изменения
  - Атомарные типы:
    - AtomicBoolean
    - AtomicInteger
    - AtomicLong
    - AtomicReference
    - AtomicIntegerArray
    - AtomicLongArray
    - AtomicReferenceArray
    - AtomicIntegerFieldUpdater
    - AtomicLongFieldUpdater
    - AtomicReferenceFieldUpdater
    - AtomicMarkableReference
    - AtomicStampedReference
• 
• 
• 
• 
