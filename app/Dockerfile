FROM centos
ADD . /code
WORKDIR /code
RUN yum install -y https://centos7.iuscommunity.org/ius-release.rpm
RUN yum -y update
RUN yum install -y python36u python36u-libs python36u-devel python36u-pip
RUN pip3.6 install -r ./requirements.txt
CMD ["python3.6", "app.py"]
