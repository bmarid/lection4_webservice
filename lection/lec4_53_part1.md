# VT-d (Virtualization technology for directed I/O)
+ Созданная корпорацией **Intel** в дополнение к её технологии виртуализации
вычислений **(VT)**, известной под кодовым названием **Vanderpool**. Виртуализация
ввода-вывода позволяет пробрасывать (pass-through) устройства на шине **PCI** (и
более современных подобных шинах) в гостевую ОС, таким образом, что она может
работать с ним с помощью своих штатных средств. Чтобы такое было возможно, в
логических схемах системной платы используется специальное устройство
управления памятью ввода-вывода **(IOMMU)**, работающее аналогично **MMU**
(memory management unit) центрального процессора, используя таблицы страниц и
специальную таблицу отображения **DMA** (DMA remapping table — DMAR), которую
гипервизор получает от **BIOS** через **ACPI** (интерфейс управления конфигурацией
оборудования и питанием).
