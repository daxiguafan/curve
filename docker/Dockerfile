FROM opencurvedocker/curve-base:debian9
ENV TZ=Asia/Shanghai
RUN mkdir -p /curvebs /etc/curve /core
COPY curvebs /curvebs
COPY entrypoint.sh /
COPY curvebs/tools/sbin/curve_tool /usr/bin
RUN chmod a+x /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]
