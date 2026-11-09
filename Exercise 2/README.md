# Упражнение 2 -- Configuring GRE

Алекс Цветанов, фак. № 371326005  
Преподавател: д-р Йонка Ганчева  
Дата: 09.11.2026 г.

- `report.tex` / `report.pdf`: лабораторен протокол на български с екранни снимки.
- `cisco/Configuring GRE.pka`: завършена задача, **100/100**, 12/12 елемента.
- `configs/`: приложените команди на RA и RB.
- `evidence/results.txt`: препис на наблюдаваните резултати.
- `images/`: топология, маршрутизация, ping, traceroute и оценка.

PCB достига PCA с 4/4 отговора без загуби; traceroute от PCA към PCB преминава през 192.168.1.1 и 10.10.10.2.

Компилиране от тази папка с MacTeX/TeX Live:
```sh
pdflatex -interaction=nonstopmode -halt-on-error report.tex
pdflatex -interaction=nonstopmode -halt-on-error report.tex
```
