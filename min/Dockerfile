FROM cefore/base
WORKDIR /cefore/cefore
RUN ./configure
RUN make
RUN make install
RUN make clean
RUN ldconfig
WORKDIR /cefore/cefpyco
RUN cmake .
RUN make
RUN make install
ENV USER=root
COPY ./entrypoint.bash /cefore
ENTRYPOINT ["bash", "/cefore/entrypoint.bash"]
