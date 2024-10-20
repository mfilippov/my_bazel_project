load("//:my_rule.bzl", "my_rule")
my_rule(
	name = "hello",
	content = "Hello Bazel!",
)

genrule(
   name = "convert_to_uppercase",
   srcs = ["input.txt"],
   outs = ["output.uppercase.txt"],
   cmd = "tr '[:lower:]' '[:upper:]' < $(SRCS) > $(OUTS)",
)
