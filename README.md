baseline v1 model
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
<!-- - v3.0
    - even bigger DNN arch
    - early stop callback
    - adjustable lr callback with patience=1
    - batch=16
    - performance:
        Acc:  0.35125448028673834
        Prec:  0.30829333245525525
        F1:  0.310698438266335     -->
- v3.1
    - even bigger DNN arch
    - adjustable lr callback with patience=3
    - batch=16
     - performance:
        Acc:  0.5340501792114696
        Prec:  0.5438670690103827
        F1:  0.513753722803421


tl v1 model
- efficient net b0
- batch=16
- adjustable lr callback with patience=2
