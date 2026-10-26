# Упражнение 1

Алекс Цветанов, фак. № 371326005  
Преподавател: д-р Йонка Ганчева  
Дата: 26.10.2026 г.

- `report.tex` / `report.pdf`: общ лабораторен протокол на български за двете задачи от Упражнение 1.
- `cisco/Packet Tracer - Skills Integration Challenge.pka`: завършена основна задача, **100/100**.
- `cisco/Packet Tracer - Configuring PAP and CHAP Authentication.pka`: предходната задача, **90/90**.
- `cisco/Packet Tracer - Troubleshooting PPP with Authentication.pka`: завършена диагностична задача, **100/100**. Началният вариант е запазен като `Packet Tracer - Troubleshooting PPP with Authentication -- initial.pka`.
- `configs/troubleshooting/`: корекциите по R1, R2 и R3 в диагностичната задача.
- `evidence/troubleshooting-results.txt`: резултатите от нея, включително ping и traceroute.
- `configs/`: приложените команди за основната задача; това не са пълни running-config exports.
- `evidence/results.txt`: транскрипция на наблюдаваните резултати от Packet Tracer.
- `images/tu_logo.png`: логото от предоставения образец за оформление.

Отваряне на PKA файловете: Cisco Packet Tracer 9.0.1. Лабораторни пароли по условие: `cisco` за конзола, `class` за privileged EXEC.

Компилиране на протокола (от тази папка, с TeX Live/MacTeX):

```sh
pdflatex -interaction=nonstopmode -halt-on-error report.tex
pdflatex -interaction=nonstopmode -halt-on-error report.tex
```

Образец за оформление: [mcse05-rdma-coursework](https://github.com/Alex-Tsvetanov/mcse05-rdma-coursework/blob/main/main.pdf). Използвани са неговите полета, шрифт, заглавна страница и номерация. Личните данни са заменени с изрично предоставените за този протокол.

## Проверки

PC15 и PC25 достигат Web по IPv4 и IPv6 с 4/4 отговора в крайните ping тестове. ICMP Simple PDU от L25, R1, R2 и S1 към Web е успешен. Първите неуспешни опити са запазени в текстовите резултати. IPv6 тест от L25 и ping от Laptop в предходната задача не са изпълнени.

PC1 и PC3 достигат 209.165.200.2 с 4/4 отговора и успешен traceroute през четири стъпки в диагностичната задача.

В `images/` са включени шест изрязани екранни снимки от Packet Tracer: топология, оценка и проверки на свързаността за всяка задача. Снимките са добавени в общия протокол с надписи на български.
