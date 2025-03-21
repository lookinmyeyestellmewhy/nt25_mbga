*  for testing time and save imgs: "python test_demo.py --data_dir ../test_infer --save_dir ../results --model_id 36 --include_test --save_img"
* for testing time and calculating parameters: "python test_demo.py --data_dir ../test_infer --save_dir ../results --model_id 36 --include_test"
** the command above  will cost incorrect flops calculation because of the some unsupported  operator of FlopCountAnalysis. If you want to get the correct flops, please use the command below: "python test_demo.py --data_dir ../test_infer --save_dir ../results --model_id 36 --include_test --not_use_fast_op" (OR just set "use_fast_op" to False in network's definition), but the running time is slower than not using "--not_use_fast_op".

