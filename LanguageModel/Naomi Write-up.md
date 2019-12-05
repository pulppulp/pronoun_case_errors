### Naomi Write-up

#### Devide the bigram into aX and Xb

1. Total number bigram: 44071
2. aX: 1288 Xb: 1289 (X = pronoun not include you it) aXb: 1289
3. in aX: when X is NOM: 926;205, X is ACC: 362;143
4. in Xb: when X is NOM: 926;288, X is ACC: 363;146
5. in aXb: when X is NOM: 926;549, X is ACC: 363;243
6. in aX, Nom - Acc: 526; 108, Acc - Nom:344; 90 ; type in Xb, Nom - Acc: 771;152, Acc-Nom: 208;78
7. aX rate: 526/926 = 0.57 108/205 = 0.53 344/362 = 0.95 90/143 = 0.63
8. Xb rate: 771/926 = 0.83 152/288 = 0.53 208/288 = 0.72 78/146 = 0.53

#### Feedforward Neural Network

1. aX: intrinsic: 0.7635, extrinsic: 0.87764
2. Xb: intrinsic: 0.7248, extrinsic: 0.89558
3. aXb: intrinsic: 0.8023 extrinsic: 0.86437

#### Desicion Tree

1. aX: intrinsic: NB:0.88235 Tree: 0.88234 extrinsic: NB: 0.92213 Tree: 0.920703
2. Xb: intrinsic: NB: 0.8916 Tree: 0.879 extrinsic: NB: 0.91388 Tree: 0.913168
3. aXb: intrinsic: NB: 0.87616 Tree: 0.87925 extrinsic: NB: 0,874 Tree: 0,88589



### Eve Write up

#### Devide the bigram into aX and Xb

1. Total number of bigram: 52988
2. aX:
3. in aX: X is Nom: 1221;206  X is Acc: 525;166
4. in bX: X is Nom: 1217; 325 X is Acc: 527;170
5. in aXb: X is Nom: 1221;614 X is Acc: 527;299
6. in aX, Nom - Acc: 629; 103, Acc - Nom:463;101 ; type in Xb, Nom - Acc: 936;180, Acc-Nom: 299;102
7. aX rate: 629/1221=0.52 103/206=0.5 463/525=0.88 101/166=0.61
8. Xb rate: 936/1217=0.77 180/325=0.55 299/527=0.57 102/170=0.6

#### Feedforward Neural Network

1. aX: intrinsic: 0.89714, extrinsic: 0.909217
2. Xb: intrinsic: 0.80857, extrinsic: 0.877094
3. aXb: intrinsic: 0.89428 extrinsic: 0.76821

#### Desicion Tree

1. aX: intrinsic: NB:0.96338 Tree: 0.0.96198 extrinsic: NB: 0.935193 Tree: 0.935193
2. Xb: intrinsic: NB: 0.9016018 Tree: 0.897025 extrinsic: NB: 0.88363 Tree: 0.887890
3. aXb: intrinsic: NB: 0.86956 Tree: 0.867276 extrinsic: NB: 0.90160 Tree: 0.90255



### Nina Write up

#### Devide the bigram into aX and Xb

1. Total number of bigram: 52988
2. aX:
3. in aX: X is Nom: 7778;500  X is Acc: 3159;543
4. in bX: X is Nom: 7766;1094  X is Acc: 3175; 516
5. in aXb: X is Nom: 7780;2449 X is Acc: 3176;1398
6. in aX, Nom - Acc: 2682; 218, Acc - Nom:2223;259 ; type in Xb, Nom - Acc: 3813;442, Acc-Nom: 1218;215
7. aX rate: 2682/7778=.34 218/500=0.44 2223/3159=0.70 259/543=0.48
8. Xb rate: 3813/7766=0.49 442/1094=0.40 1218/3175=0.38 215/516=0.42

#### Feedforward Neural Network

1. aX: intrinsic: 0.973, extrinsic: 0.8919
2. Xb: intrinsic: 0.88321, extrinsic: 0.86552
3. aXb: intrinsic: 0.96629 extrinsic: 0.838

#### Desicion Tree

1. aX: intrinsic: NB:0.97079 Tree: 0.97188 extrinsic: NB: 0.9022 Tree: 0.8903
2. Xb: intrinsic: NB:0.8868 Tree: 0.88499 extrinsic: NB: 0.88363 Tree: 0.887890
3. aXb: intrinsic: NB: 0.91639 Tree: 0.9142 extrinsic: NB: 0.84024 Tree: 0.836419

