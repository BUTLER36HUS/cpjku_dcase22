# 一些想法
- 能否使用Masked Auto-Encoder的方法来训练一个预测waveform或是spectrogram的encoder-decoder。然后再利用这个encoder去训练一个分类的decoder了？
    - 用waveform
        - 我们真的需要进行SFT吗？将1d的波形文件分解成2d的spectrogram对于transformer模型来说真的是帮助吗？
            - 在cnn角度来讲是的，但是transformer也是吗？
    - 用spectrogram

## Why?
- 训练auto-encoder并不需要strongly annotated数据，甚至不需要weakly annotated数据。只需要相关的音频文件就行了

## Difficulities
- auto-encoder not gauranteed to converge
- expensive and time-consuming
