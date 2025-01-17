---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# О проекте

## **Система наведения направленной антенны без использования системы навигации для увеличения дальности связи дронов**

**BRICS2024: UAS Challenge,** Казань



**Среда разработки:**&#x20;

\- Frontend: JavaScript (Vue, Vuetify)&#x20;

\- Backend: Python (FastAPI, aiortc)&#x20;

\- Антенна Трекер: C lang&#x20;

**Оборудование:**&#x20;

\- Дрон: Клевер, Foxeer Lollipop 4, TBS UNITY PRO32 5G8 HV

\- Сервер: Raspberry Pi&#x20;

\- Антена Трекер: Arduino, SkyDroid PF V 5.8G



**Цель проекта:** Разработка и реализация системы, которая повышает эффективность работы антенны направленного типа за счет автоматической коррекции направления в сторону БПЛА.

**Актуальность:** Потеря связи с дронами на большом расстоянии из-за ограниченного угла работы направленной антенны является распространенной проблемой в области беспилотных технологий.

### **Задачи:**

1. Создание блок-схемы проекта
2. Определение необходимых компонентов
3. Разработка алгоритма автоматической коррекции
4. Разработка прошивки микроконтроллера;
5. Разработка программного обеспечения для управления антенным трекером.
6. Разработка Frontend части проекта
7. Разработка Backend части проекта
8. Разработка электронной схемы
9. Проектирование механических элементов
10. Печать компонентов на 3D принтере
11. Сборка устройств
12. Тестирование и отладка
13. Подготовка документации
14. Подготовка презентации

### **Основные функции:**

* Автоматическая настройка направления: система отслеживает сигнал от дрона и поворачивает антенну в сторону максимальной амплитуды сигнала;
* Самостоятельная работа: работает на собственном программном обеспечении, не требует GPS или компаса для работы, питается от аккумуляторов;
* Портативность: легко перемещается и устанавливается в различных местах;
* Универсальность: совместима с различными типами беспилотных систем и антенн;

**Преимущества:**

* &#x20;Увеличение дальности связи: позволяет поддерживать стабильный сигнал с дронами на значительном расстоянии;
* Повышение надежности: минимизирует риск потери связи с дроном, что особенно важно для проведения критических операций
* Автономность: работает от аккумулятора, не требует питания от высоковольтной сети переменного тока, что позволяет использовать систему в различных условиях.
* Простая интеграция: легко подключается к различным беспилотным системам, не требуя сложной настройки.

### Нововведения:

В представленном устройстве мы решили ряд проблем, характерных для готовых антенных трекеров.



| Проблема                                                                                                             | Наше решение                                                                                                                                                                                                                                                                                                                                                                          |
| -------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Использование модулей GPS и компаса для точного позиционирования дрона в пространстве и «нацеливания» антенны.       | Создание системы отслеживания дрона, которая использует только качество сигнала от дрона для корректировки поворота антенны. Это позволяет исключить необходимость использования GPS и компаса как на наземном модуле антенного трекера, так и на самом дроне.                                                                                                                        |
| Ограниченные возможности готовых программных решений, а также отсутствие широко используемых отечественных аналогов. | <p>Разработано собственное программное обеспечение для микроконтроллера и веб-интерфейс для взаимодействия с дроном. Это позволяет:</p><ul><li>получать видеопоток с дрона;</li></ul><ul><li>автоматически находить дрон с максимальным уровнем сигнала;</li></ul><ul><li>искать дрон по известной частоте видеосигнала;</li></ul><ul><li>выводить качество сигнала (RSSI).</li></ul> |
| Использование готовых программных решений могло бы привести к проблемам с правообладателем и авторским правом.       | Весь программный код и схема устройства были разработаны с нуля, что обеспечивает полную свободу в разработке и модификации устройства.                                                                                                                                                                                                                                               |

### **Целевая группа:**

* Операторы беспилотников: операторы, работающие с дронами на больших расстояниях, например, для сельского хозяйства, инспекции, мониторинга, доставки;
* Производители беспилотных систем: производители дронов могут интегрировать систему в свои продукты для повышения дальности связи;
* Исследователи и разработчики: исследовательские группы и компании, работающие над разработкой автономных систем, могут использовать систему для повышения надежности связи

### **Дополнительные преимущества:**

* Уменьшение затрат: увеличивает эффективность использования дронов, сокращает затраты, т.к. не требует модуля GPS и компаса как на устройстве, так и на летательном аппарате;
* Повышение безопасности: улучшает связь с дронами, что позволяет операторам эффективно контролировать их работу
* Открытие новых возможностей: позволяет использовать дроны для выполнения задач на большем расстоянии, расширяя область их применения
