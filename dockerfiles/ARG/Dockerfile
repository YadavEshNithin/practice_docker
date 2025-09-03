ARG version
FROM almalinux:${version:-9}
ARG trainer="siva_sir"
ENV COURSE="devops"
ENV trainer=$trainer
RUN echo "hello good morning ${trainer} the course is ${COURSE}" > result.txt
CMD ["sleep", "1000"]