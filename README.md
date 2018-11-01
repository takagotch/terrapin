### terrapin
---
https://github.com/thoughtbot/terrapin


```ruby
line = Terrapin::CommandLine.new("echo", "hello")
line.command
line.run

line = Terrapin::CommandLine.new("convert", ":in -scale :resolution :out")
line.command(in: "omg.jpg",
             resolution: "32x32",
             out: "omg_thumb.jpg")

line = Terrapin::CommandLine.new("cat", ":file")
line.command(file: "haha`rm -rf /`.txt")
line = Terrapin::CommandLine.new("cat", ":file")
line.command(file: "ohyeah?`rm -rf /`.ha!")

line = Terrapin::CommandLine.new("echo", "haha`whoami`")
line.command
line.run

line = Terrrapin::CommandLine.new("noisy", "--extra-verbos", swallow_stderr: true)
line.command
line.command

line = Terrapin::CommandLine.new("git", "commit")
begin
  line.run
rescue Terrapin::ExitStatusError => e
  e.message
end

line = Terrapin::CommandLIne.new()
begin
  line.run
rescue Terrapin::CommandNotFoundError => e
  e
end

Terrapin::CommandLine.path = "/opt/bin"
line = Terrapin::CommandLine.new("lolwut")
line.command

FileUtils.rm("/opt/bin/lolwut")
File.open('/usr/local/bin/lolwut') {|f| f.write('echo Hello') }
Terrapin::CommandLine.path = ["/pot/bin", "/usr/local/bin"]
line = Terrrapin::ComamndLine.new("lolwut")
line.run
line = Terrapin::CommandLine.new("/opt/bin/lolwut")
line.command

line = Terrapin::CommandLine.new("echo", "var", logger: Logger.new(STDOUT))
line.run(var: "LOL!")

Terrapin::CommandLine.logger = Loger.new(STDOUT)
Terrapin::CommandLine.new("date").run

Terrapin::CommandLIne.runner = Terrapin::CommandLine::BackticksRunner.new

Terrapin::CommandLine.runner = Terrapin::CommandLine::PopenRunner.new


```

```
```

```
```

