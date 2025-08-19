some random notes

Video 1: What's new in C# 13 
- CollectionExpression.cs
- IList, IDirectionary
	- What if keys are the same?
- Extensions for everything, besides methods
- Unions: A variable can be either type A or type B

VIdeo 2: Open Source
- History of software distribution
	- Used to buy physical Windows licences, sell when done
	- Now you almost never own the software, just subscribe to the survives
- Free Beer: Free, but there's some restrictions
- Freedom of Speech
- Open source
	- People can steal your work
	- Feel an obligation to maintain work
- Free weekend
	- Freely work as you please, no obligation

Video 3: High-Performance Computing
- Covering
	- Performance
	- Measuring applicaiton and code peformance
	- Span, ReadOnlySpanMemory
	- ArrayPool
- Performance
	- Execution Time, Throughput, Memory Allocations
	- Is contextual
	- Balance between perforamnce and readability
		- Readability is better for working with large teams, code changes often
- Optimization Cycle
	- Measure: Are the changes we're making having a positive impact
		- CPU, measuring execution time, memory allocations
		- Benchmarking
	- optimize:
		- Small changes
		- Find the bigger wins, sometimes enough is good
- Measuring perf
	- Diagnostic tools (debugging)
	- Profiling / PerfView / dotTrace / dotMemory
	- ILSpy / dotpeeek / JustDecompile
		- Intermediate Language - > executed by the JIT]
	- Production metrics and monitoring
		- APM Agent for .NET
- Benchmark
	- JIT: there's different tiers: balance between time to deliver, optimize performance as it makes sense. SIMD
	- AOT: I promise it will be ready by then
	- Compare on different platforms, architectures, JIT versiona nd GC Modes
		- Different GC levels
	- benchmarkdotnet.org

