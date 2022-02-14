# Anchor not defined example

pseudomuto/protoc-gen-doc:1.5.0 function 'anchor' not defined example.

## Error example

template: Text Template:2: function "anchor" not defined

```sh
TAG=1.5.0
docker run --rm \
	-v $(PWD)/src/docs:/out:rw \
	-v $(PWD)/src/protos:/protos:ro \
	-v $(PWD)/src/templates:/templates:ro \
	pseudomuto/protoc-gen-doc:$(TAG) \
    --doc_opt=/templates/example.tmpl,example.md ./protos/example.proto
```

If clone https://github.com/pseudomuto/protoc-gen-doc repository and build Dockerfile localy and change TAG from "1.5.0" to "local" example.md was builded.
