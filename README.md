# braindump
Decode EEG data files produced by Neuroscope

sample command lines:

./neurolator /Users/xxx/xxx/ProjectEmbReact_M508_20170203_SleepPost_Robin.dat 0 6 0 | ./ffmpeg -y -f s16le -ar 20000 -ac 1 -i - EmbReact20170203_sleepPost-0.aiff

./neurolator /Users/xxx/hc2/ec013.529-water.dat 1 31 0 | ./ffmpeg -y -f s16le -ar 20000 -ac 1 -i - ec013-529-water-1.aiff
converts channel 1 of 31 channel dat file to a 20kHz 16bit aiff file

./neurolator /Users/xxx/Mouse12-120809-03.dat 1 90 0 | ./ffmpeg -y -f s16le -ar 20000 -ac 1 -i - Mouse12-120809-03-1.aiff
