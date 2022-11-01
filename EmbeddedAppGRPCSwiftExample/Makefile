generate-swift-protos:
	mkdir -p generated
	protoc \
	protos/Example.proto \
	-I. \
	--plugin=`which protoc-gen-swift` \
	--swift_opt=Visibility=Public \
	--swift_out=generated \
	--plugin=`which protoc-gen-grpc-swift` \
	--grpc-swift_opt=Visibility=Public \
	--grpc-swift_out=generated
.PHONY: generate-swift-protos
