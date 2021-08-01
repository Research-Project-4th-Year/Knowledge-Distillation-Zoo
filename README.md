#knowledge distillation 2015

python -u train_kd.py --save_root "./results/soft-target/"  --t_model "./results/base/base-c10-r20/model_best.pth.tar"  --s_init "./results/base/base-c10-r20/initial_r20.pth.tar"  --data_name cifar10  --num_class 10  --t_name resnet20  --s_name resnet20  --kd_mode st  --lambda_kd 0.1 --note soft-target-c10-r20-r20 --epochs 20