ARG BUILD_FROM
FROM $BUILD_FROM

# Initialize
 RUN   apk update \                                                                                                                                                                                                                        
  &&   apk add ca-certificates wget \                                                                                                                                                                                                      
  &&   update-ca-certificates \   
  &&   apk add --no-cache python3

# Copy data for add-on
COPY run.sh /
RUN chmod a+x /run.sh

CMD [ "/run.sh" ]