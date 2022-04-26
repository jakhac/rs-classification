<!-- baseline v1 model
- batch=32
- standard DNN arch
- performance:
    Acc:  0.31899641577060933
    Prec:  0.35939284729607307
    F1:  0.31495155488566473

baseline v2 model
- enhanced DNN arch: more filters in later convs
- batch=32
- deal with imbalance:
    - apply class weights during training
    - more data by ImageDataGenerator
- performance:
    Acc:  0.4121863799283154
    Prec:  0.41809734744731514
    F1:  0.3882773348005602


baseline v3 model
- v3
- even bigger DNN arch
- batch=16
- performance:
    Acc:  0.5340501792114696
    Prec:  0.5438670690103827
    F1:  0.513753722803421

- v3.2
- adjusted dropout layer 0.2 0.3 0.5


tl v1 model
- efficient net b0
- batch=16
- adjustable lr callback with patience=2
- performance:
    Acc:  0.7706093189964157
    Prec:  0.8031684363196874
    F1:  0.7637736415980427 -->


TODO
- sort class distribution
- explain choice of efficient net
