
IOP_BIN = btstack.irx
IOP_OBJS = btstack.o imports.o exports.o
IOP_OBJS_DIR = obj.btstack/

IOP_OBJS := $(IOP_OBJS:%=$(IOP_OBJS_DIR)%)

IOP_CFLAGS += -Wall -fno-builtin -DUSE_SMSUTILS
IOP_LDFLAGS += -s

all: OBJ_DIR $(IOP_BIN)

clean:
	rm -f $(IOP_BIN) $(IOP_OBJS)

rebuild: clean all

OBJ_DIR:
	mkdir -p $(IOP_OBJS_DIR)

include $(PS2SDK)/Defs.make
include ../Rules.make
