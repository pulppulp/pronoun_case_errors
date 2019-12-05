Peter Write-up

#### Get Peter's mother's trigram and bigram 

1. ('d', 'you') — 'd' is likely to be did, had, would...
2. There are huge amount of 'you' and 'it'

#### Devide the bigram into aX and Xb

1. Total number bigram: 4172
2. aX: 2095 Xb: 2095 — probably there are overlapped XX
3. in aX, when X is NOM: 447;161, X is ACC: 202;93, X is you: 1046;165, X is it: 400;126
4. in Xb, when X is NOM: 444;209, X is ACC: 205;103, X is you: 1042;200, X is it: 404;113
5. turn all pronouns into X in aX and Xb framework
6. Calculate Accuracy: 

for aX: unique NOM type= 93, token=297   unique ACC type = 63, token = 192

for Xb: unique NOM type = 128, token = 375     unique ACC type = 62, token = 132



#### Devide the trigram into aXb

1. Total number of trigram: 5572
2. aXb: 2104, X is NOM: 447;320  ACC: 205;142, YOU: 1047;562, it: 405;265
3. unique NOM type: 301, token: 447 ACC type: 126, token: 205



#### Feedforward Neural Network

aX: 100 hidden layer, intrinsic accuracy 0.70 (80% train, 20% test) extrinsic accruracy (0.77 train adults, test Peter)

aXb: 100 hidden layer, intrinstic accuracy 0.76 (80% train, 20% test) extrinsic accuracy (80% train, test Peter — 0.782022, 100% train, test Peter — 0.7825545)

#### Decision Tree

aX

aXb: 100% train, test Peter — 0.835//, 80%train, 20% test — 0.828



