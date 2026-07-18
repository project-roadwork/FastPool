# FastPool
Derived from: ObjectPool by qaltx (under the MIT License)
	ObjectPool: https://github.com/notqaltx/ObjectPool.git

   	Modifications:
   		- Replaced class/metatable-based pools with closure-based pools
   		- Removed UsageMetrics table storage; metrics are stored as individual numbers
   		  and are only assembled into a table when requested
   		- Added lifecycle functions: Destroy(), Reset(), and Clear()
   		- Added utility functions: TogglePooling() and GetMetrics()
		- Renamed: ObjectPool.new() -> FastPool()
		- Renamed: Pool:GetObject() -> Pool.Get()
		- Renamed: Pool:ReturnObject() -> Pool.Return()
		- Tracks number of reused objects
		- Removed ActiveObjects table in order to reduce memory usage with many objects
		- Removed HierarchicalPools table
		- No longer traditional object-oriented programming (OOP)
		- Removed mutex
		- No longer Instance-centric
		- New destroy() argument
		- Removed debugger and signal module

## License
MIT License or Apache License 2.0 WITH LLVM-exception
