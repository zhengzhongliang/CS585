FROM python:2
ADD DNC_tensorflow_master/ DNC_tensorflow_master/
ADD DNC_tensorflow_master/tasks/babi/data/ data/
ADD DNC_tensorflow_master/tasks/babi/checkpoints/ checkpoints/
RUN pip install tensorflow==0.12.0
RUN pip install numpy==1.11.0
CMD [ "python", "./DNC_tensorflow_master/tasks/babi/test.py" ]

