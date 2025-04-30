
FROM eclipse-temurin:8-jdk-jammy

WORKDIR /app

COPY src ./src

RUN find src -name "*.java" > sources.txt \
    && mkdir -p out \
    && javac @sources.txt -d out

CMD ["java", "-cp", "out", "CaseStudy.question1.Main"]
