

OBJ_DIR=../../release/obj

INCLUDES=		-Iincludes \
						-I../includes \
						-I../debug/includes \
						-I../libs/includes  \
						-I../mylibrary/includes \
						-I../memory/includes \
						-I../kernel/includes \
						-I../rmode/includes 


CPP_SRC=file_system.cpp \
				my_file_system.cpp

CPP_OBJ_FILE=$(CPP_SRC:.cpp=.o)

CPP_OBJ=$(addprefix $(OBJ_DIR)/, $(CPP_OBJ_FILE))


all: $(CPP_OBJ)

$(OBJ_DIR)/%.o: %.cpp
	$(CPP_CC) $(INCLUDES) $< -o $(OBJ_DIR)/$@
	

clean: 
	rm *.o


