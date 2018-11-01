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

line = Terrapin::CommandLine.new("noisy", "--extra-verbose", swallow_stderr: true)
line.command()
line.run()

line = Terrrapin::CommandLine.new()
line.command

line = Terrapin::CommandLine.new()
begin
rescue
end

line = Terrapin::CommandLine.new(
begin
rescue Terrapin::ExitStatusError => e
end

line = Terrapin::CommandLIne.new()
begin
rescue Terrapin::CommandNotFoundError => e
end

Terrapin::CommandLine.path = ""
line = Terrapin::CommandLine.new()
line.command

FileUtils.rm()
File.open() {}
Terrapin::CommandLine.path = []
line = Terrrapin::ComamndLine.new()
line.run

line = Terrapin::CommandLine.new()
line.command

line = Terrapin::CommandLine.new()
line.command

line = Terrapin::CommandLine.new()
line.run()

Terrapin::CommandLine.logger = Loger.new()
Terrapin::CommandLine.new().run

Terrapin::CommandLIne.runner = Terrapin::CommandLine::BackticksRunner.new

Terrapin::CommandLine.runner = Terrapin::CommandLine::PopenRunner.new


```

```
```

```
```

