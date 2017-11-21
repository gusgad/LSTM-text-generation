# LSTM Song Generation

Generating random song lyrics with an LSTM network after training on a 1M character corpus of [song lyrics](https://www.kaggle.com/mousehead/songlyrics/data). Training takes 2 hours to converge on Nvidia Titan X and almost 1.5 days with a Quad Core CPU.


Results so far:
* LSTM layers: 128, Dense(50), Softmax; Window: 40, stride: 3 - 1.1538 (30 epochs)
* LSTM layers: 128, Dense(128), Dropout(0.5), Dense(50), Softmax; Window: 40, stride: 3 - 1.2812 (30 epochs)


Given a sentence "Gabriele loves dancing\nall day and night" with a training loss of 1.1538, the network outputs something as the following:
`gabriele loves dancing`
`all day and night, girls ah`
  
`oh, she surveted down the fear and i follow`
`the best to watch it up and maybe some time`
  
`a dicty flien in the tracch fire`
`what a could on the dark`
  
`my shoo say where the cold of christmas sush`
`yeah burns and was the tail, you're here, no more`
  
`the acay on a sush farm`
`to stay i'm stupir`
`beaine comes`
  
`gonna be a longed are over`
`kissest are this`
`here we'll see well i les exptain`
`i can't ever two to day`
  
`how can be unde strome when she stop me, now`
