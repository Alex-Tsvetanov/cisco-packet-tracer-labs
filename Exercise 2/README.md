# Упражнение 2 -- Configuring GRE и Troubleshooting GRE

Алекс Цветанов, фак. № 371326005  
Преподавател: д-р Йонка Ганчева  
Дати: 09.11.2026 г. и 18.11.2026 г.

- `report.tex` / `report.pdf`: лабораторен протокол на български с екранни снимки.
- `cisco/Configuring GRE.pka`: завършена задача, **100/100**, 12/12 елемента.
- `cisco/Troubleshooting GRE.pka`: завършена диагностика, **100/100**, 5/5 елемента.
- `configs/`: приложените команди на RA и RB.
- `evidence/results.txt`: препис на наблюдаваните резултати.
- `images/`: топология, маршрутизация, ping, traceroute и оценка.

PCB достига PCA с 4/4 отговора без загуби; traceroute от PCA към PCB преминава през 192.168.1.1 и 10.10.10.2.

Компилиране от тази папка с MacTeX/TeX Live:
```sh
pdflatex -interaction=nonstopmode -halt-on-error report.tex
pdflatex -interaction=nonstopmode -halt-on-error report.tex
```

Troubleshooting GRE: поправени са адресите на RA, неговият статичен маршрут и крайните точки на RB. Краен ping PCB към PCA: 4/4, RTT 22/28/33 ms. Traceroute: 172.31.0.1 → 192.168.1.2 → 172.31.1.2. Подробности: `evidence/troubleshooting-results.txt`.
