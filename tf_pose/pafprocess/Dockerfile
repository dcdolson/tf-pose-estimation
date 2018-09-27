FROM openpose:preprocess

RUN apt-get update && apt-get install -y swig

RUN  cd /root/tf-openpose/tf_pose/pafprocess \
 && swig -python -c++ pafprocess.i

RUN cd /root/tf-openpose/tf_pose/pafprocess/ \
 && python3 setup.py build_ext --inplace

