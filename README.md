# How to reproduce
1) Get the CARML CLI interface from here - https://github.com/carml/carml-jar
  - Clone the repo and run "mvn clean package"
  - This will generate the file called: `carml-jar-1.0.0-SNAPSHOT-0.4.1.jar`
2) Clone this repo
3) Copy the *.jar file from step 1 into the directory of this repo
4) Execute `run.sh`

Expeced error message:
`
./run.sh
io.carml.engine.RmlMapperException: Could not resolve source for logical source: blank node resource _:c9fc2573062744ce8f64e8de6f5e105d1 in:

[] a rml:LogicalSource;
  :causedException "<<<<<<<<<<<<<";
  rml:source "characters.json";
  rml:iterator "$.characters[*]";
  rml:referenceFormulation ql:JSONPath .

    at io.carml.engine.RmlMapper.lambda$resolveSource$3(RmlMapper.java:133)
`