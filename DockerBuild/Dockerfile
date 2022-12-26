FROM ubuntu:16.04

RUN apt-get update
RUN apt-get install build-essential -y
RUN apt-get -y install cmake git
RUN apt-get -y install libpng-dev libjpeg-dev libtbb-dev libtiff-dev libeigen3-dev wget

# # download opencv-2.4.11
# RUN wget http://downloads.sourceforge.net/project/opencvlibrary/opencv-unix/2.4.11/opencv-2.4.11.zip
# RUN unzip opencv-2.4.11.zip
# RUN cd opencv-2.4.11
# RUN mkdir release
# RUN cd release
 
# # compile and install
# RUN cmake -G "Unix Makefiles" -D CMAKE_CXX_COMPILER=/usr/bin/g++ CMAKE_C_COMPILER=/usr/bin/gcc -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local -D WITH_TBB=ON -D BUILD_NEW_PYTHON_SUPPORT=ON -D WITH_V4L=ON -D INSTALL_C_EXAMPLES=ON -D INSTALL_PYTHON_EXAMPLES=ON -D BUILD_EXAMPLES=ON -D WITH_QT=ON -D WITH_OPENGL=ON -D BUILD_FAT_JAVA_LIB=ON -D INSTALL_TO_MANGLED_PATHS=ON -D INSTALL_CREATE_DISTRIB=ON -D INSTALL_TESTS=ON -D ENABLE_FAST_MATH=ON -D WITH_IMAGEIO=ON -D BUILD_SHARED_LIBS=OFF -D WITH_GSTREAMER=ON ..
# RUN make all -j4 # 4 cores
# RUN sudo make install

# docker build -t minhnd/base_ubuntu .
# docker run --rm --name base_minh -it --mount type=bind,source="$(pwd)",target=/texturing/ lehotcd/base_ubuntu bash 

#WORKDIR mvs-texturing/
#RUN mkdir build && cd build && cmake .. && make
#RUN ls apps/
#RUN ls apps/texrecon
#RUN ./build/libs/tex/libtex.a