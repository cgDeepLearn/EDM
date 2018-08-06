# 第五章 数字音频

为了防止某些位置上的音频信号没有被"测量"到，必须保证采样频率大于波形频率的两倍。
这个原理叫作Nyquist-Shannon采样定律。它表明了要在数字域内精确重现波形，每个波形周期至少要有两个采样点。
人耳的听觉范围的最高频率约为20kHz，那么采样率应超过它的两倍。

通常音频CD的采样率是44.1kHz = 20KHz + 4100Hz(确保采样频率大于两倍，多余的频率用于抗混叠滤波器)。还有更高的采样率。

## 采样精度

对于数字录音系统而言，比特数决定了测量波形音量的模拟电压数量，实际上也决定了动态范围。

从技术上讲，动态范围指的是由音频设备产生的静态噪声(也就是本底噪声)与可允许的最大不失真电平之间的比值。
对于音乐来说，动态范围是指最静部分与最响部分的差值。

本质上讲，如果录音时采用地采样精度，就只能保留少量的动态，导致声音最响部分与本底噪声之间的差变得很小，因此背景噪声就会更明显。

量化噪声。

对于实际应用来说，尽管CD只有16-Bit，但在数字录音、编辑和处理的过程中采用24-Bit精度，当最后声音下降到16-Bit精度并刻录CD时，量化噪声将大幅减少。

降低音频的采样精度也叫作“抖动”(`Dithering`).`Apogee`的抖动算法被公认为是非常优秀的。

最后，无论采样精度是多少，重要的是声卡或数字录音机中的转换器品质要好，并且信号录制的电平要尽可能得大(在不失真的前提下)。如果信噪比比较低，当提升录制信号的增益时，本底噪声也会以同样的幅度被提升。

要注意选取合适的录音增益，但也不要让信号过大造成削波失真。

通过在信号源和录音设备之间串联压缩器可以实现动态限制。
压缩器压缩某个阈值范围以上的信号，因此减小了可能导致削波的峰值信号并保证了相对高的录音电平。