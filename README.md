This is a test repo for versioned go.
There's nothing useful here.

	v0.0.0 - has pkg/p.go
	v0.0.1 - has go.mod
	
	v1.0.0 - has pkg/p.go
	v1.0.1 - has go.mod
	v1.0.2 - has submod/pkg/p.go
	v1.0.3 - has submod/go.mod
	submod/v1.0.4 - same
	submod/v1.0.5 - add requirement on v1.1.0
	v1.1.0 - add requirement on submod/v1.0.5
	
	v2.0.0 - has pkg/p.go
	v2.0.1 - has go.mod with v2 module path
	v2.0.2 - has go.mod with v1 (no version) module path
	v2.0.3 - has v2/go.mod with v2 module path
	v2.0.5 - has go.mod AND v2/go.mod with v2 module path
	