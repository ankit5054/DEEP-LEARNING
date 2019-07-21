# DEEP-LEARNING
![1_goFgCUHprcroxSLZvROjpg](https://user-images.githubusercontent.com/39160589/61589055-06a99a80-abcb-11e9-8b97-2f5339eba6fe.jpeg)


## Multi Layer Perceptron (MLP)
I have applied the Neural Network on the MNIST dataset<br>

ABBREVATIONS <BR>
1.BN-> BATCH NORMALISATION<br>
2.DP-> DROPOUTS<br>
3.IP-> INPUT LAYER<br>
4.OP-> OUTPUT LAYER<br>

### FIRST MODEL
NO. OF HIDDEN LAYERS: 2<br>
ARCHITECTURE OF MODEL: IP->400->BN->DP->150->BN->DP->OP<br>
Categorical Crossentropy Loss: 0.0617 <br>
ACCURACY: 98.14%<br>

### SECOND MODEL
NO. OF HIDDEN LAYERS: 3<br>
ARCHITECTURE OF MODEL: IP->600->BN->DP->300->BN->DP->250->BN->DP->OP<br>
Categorical Crossentropy Loss: 0.0585  <br>
ACCURACY: 98.37%<br>

### THIRD MODEL
NO. OF HIDDEN LAYERS: 5<br>
ARCHITECTURE OF MODEL: IP->600->BN->DP->500->BN->DP->400->BN->DP->300->BN->DP->250->BN->DP->OP<br>
Categorical Crossentropy Loss: 0.0601  <br>
ACCURACY: 98.32%<br>

### FOURTH MODEL
NO. OF HIDDEN LAYERS: 5 ONLY WITH DROPOUTS<br>
ARCHITECTURE OF MODEL: IP->700->DP->550->DP->390->DP->290->DP->670->DP->OP<br>
Categorical Crossentropy Loss: 0.6135  <br>
ACCURACY: 74.38%<br>

### FIFTH MODEL
NO. OF HIDDEN LAYERS: 4 WITH ALTERNATIVE DROPOUTS<br>
ARCHITECTURE OF MODEL: IP->790->390->DP->290->670->DP->OP<br>
Categorical Crossentropy Loss: 0.469  <br>
ACCURACY: 82.42%<br>


## Convolutional Neural Network

ABBREVATIONS <br>
1.BN-> BATCH NORMALISATION<br>
2.DP-> DROPOUTS<br>
3.IP-> INPUT LAYER<br>
4.OP-> OUTPUT LAYER<br>
5.FL-> FLATTEN LAYER <br>
6.CN-> CONVOLUTIONAL LAYER<br>
7.PL-> MAX POOLING  <br>
8.DN-> DENSE LAYER<br>

### FIRST MODEL
NO. OF HIDDEN LAYERS: 3<br>
ARCHITECTURE OF MODEL: IP->CN->DP->CN->CN->PL->DP->FL->DN->DP->DN<br>
Categorical Crossentropy Loss: 0.02223 <br>
ACCURACY: 99.31%<br>

### SECOND MODEL
NO. OF HIDDEN LAYERS: 5<br>
ARCHITECTURE OF MODEL: IP->CN->DP->BN->CN->PL->DP->CN->PL->BN->DP->CN->DP->BN->PL->FL->DN->DP->DN->OP<br>
Categorical Crossentropy Loss: 0.0969 <br>
ACCURACY: 98.25%<br>

### THIRD MODEL
NO. OF HIDDEN LAYERS: 7<br>
ARCHITECTURE OF MODEL: IP->CN->DP->BN->PL->CN->BN->DP->PL->CN->DP->BN->PL->CN->BN->DP->CN->BN->DP->PL->CN->DP->BN->PL->CN->BN->DP->PL->FL->DN->DN->OP<br>
Categorical Crossentropy Loss: 0.0603 <br>
ACCURACY: 98.48%<br>

### FOURTH MODEL
NO. OF HIDDEN LAYERS: 3(NO BN AND DP)<br>
ARCHITECTURE OF MODEL: IP->CN->CN->CN->PL->FL->DN->DN<br>
Categorical Crossentropy Loss: 0.0257 <br>
ACCURACY: 99.33%<br>


## Long Short-Term Memory (LSTM)
This Algorithm is applied on Text Data.


### FIRST MODEL
Layers: 1
Architecture: EMBEDDING->LSTM->DROPOUT->DENSE
Loss: 0.6054
Accuracy: 89.26%

### SECOND MODEL
Layers: 2
Architecture: EMBEDDING->LSTM->LSTM->DENSE 
Loss: 0.7312
Accuracy: 89.41%

