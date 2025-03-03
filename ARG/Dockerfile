ARG version
FROM almalinux:${version:-9}
ARG course="devops" \
    duration="120 min"
ENV duration=$duration
RUN echo "course is $course and duration is $duration"
CMD ["sleep", "100"]