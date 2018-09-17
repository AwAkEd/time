FROM fedora:latest
ADD ./init.sh ./
RUN yum -y install nmap-ncat && yum clean all -y
RUN chown 1001:1001 init.sh && chmod o+w init.sh
USER 1001
EXPOSE 8080
CMD ["./init.sh"]
