# Speed Estimations
Алгоритм контроля за изменением профиля потока.

Программа SpeedEstimation.exe является демонстрацией алгоритма обнаружения тренда.
В программе демонстрируется 3 графика:
1) Наличие тренда в данных(синим цветом помечена линия роста)
2) Отсутствие тренда в данных(синим цветом помечена линия роста)
3) Оценка скорости звука от расчитанного значения, синим цветом помечен график, не выходящий за порог, красным - выходящий за порог.
Непосредственно сам алгоритмы реализован в виде функции estimateDataTrend - оценка тренда, estimateSoundSpeed - оценка скорости звука в файле mainwindow.cpp. 

Метод наименьших квадратов для обнаружения тренда использован с предположением о том что, изменение профиля в выборке линейно и монотонно. 
В противном случае необходимо будет дополнительно применить линеаризацию, либо нелинейные методы оценки. 
