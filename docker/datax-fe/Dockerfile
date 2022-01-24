FROM yiluxiangbei/centos7-bigdata-datax

RUN mkdir -p /home/datax-web

COPY ./datax-admin-2.1.2.jar /home/datax-web

COPY ./datax-executor-2.1.2.jar /home/datax-web

COPY entrypoint.sh /home/datax-web

WORKDIR /home/datax-web

RUN chmod +x /home/datax-web/entrypoint.sh

ENTRYPOINT ["/home/datax-web/entrypoint.sh"]