# sessionSeven-Assignment2-


input = sc.textFile(“words.txt”)

counts = input.flatMap(lambda line: line.split(" ")).map(lambda word: (word,1)).reduceByKey(lambda a, b : a+b)

counts.collect
