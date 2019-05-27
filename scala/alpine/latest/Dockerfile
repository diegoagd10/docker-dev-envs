FROM openjdk:8-alpine

ENV SBT_VERSION 1.2.8
ENV LOCAL_HOME /usr/local
ENV SBT_HOME ${LOCAL_HOME}/sbt
ENV SBT_ZIP_FILE ${LOCAL_HOME}/sbt.zip   
ENV PATH ${PATH}:${SBT_HOME}/bin

RUN apk --no-cache add curl bash && \
  curl -o ${SBT_ZIP_FILE} https://sbt-downloads.cdnedge.bluemix.net/releases/v${SBT_VERSION}/sbt-${SBT_VERSION}.zip && \
  unzip ${SBT_ZIP_FILE} -d ${LOCAL_HOME} && \
  rm ${SBT_ZIP_FILE}