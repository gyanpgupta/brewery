FROM python:3.8
ADD . /warehouse
WORKDIR /warehouse
RUN pip install flask gunicorn
EXPOSE 5003
CMD ["gunicorn", "-w", "2", "-b", "0.0.0.0:5003", "warehouse:app"]