# OSCINF-EXAMPLE

**Step 1:**
Download files from this repository

**Step 2:**
Run the following command line to generate **oscinfexe.zip**
```bash
$ java -jar OSCINF.jar OSCINFGenerator <local directory with these files> Java8.g4 ooc-o.owl Java8.ooc-o.map 
```

**Step 3:**
Extract the directory from oscinfexe.zip generated with OSCINF.jar

**Step 4:**
Run the following command line to generate **oscinfexe.jar**
```bash
$ mvn clean compile assembly:single
```

**Step 5:**
Use the **oscinfexe.jar** to process the source code with following command line
```bash
$ java -jar oscinfexe.jar <local directory with these files> Java8.g4 ooc-o.owl query.sparql <local directory with source code>
```
