VPATH = ..
CC = gcc -mmacosx-version-min=10.9
CXX = g++ -mmacosx-version-min=10.9
CFLAGS = -fPIC -Wall -g -O3 -I../ -I../nlopt  -DWX_PRECOMP -O2 -arch x86_64  -fno-common
CXXFLAGS = $(CFLAGS) -std=gnu++11

OBJECTS = \
	treemesh.o \
	apertureplane.o \
	determineelementintersectionnew.o \
	dumpsys.o \
	errors.o \
	generateray.o \
	input.o \
	interaction.o \
	intersect.o \
	mathproc.o \
	newzstartforcubicsplinesurf.o \
	quadricsurfaceclosedform.o \
	root432.o \
	spencerandmurtysurfaceclosedform.o \
	stapi.o \
	suntoprimarystage.o \
	surface.o \
	surfacenormalerrors.o \
	surfacezatxypair.o \
	torusclosedform.o \
	raytrace.o \
	types.o \
	vshot.o


TARGET=coretrace.a

$(TARGET):$(OBJECTS)
	ar rs $(TARGET) $(OBJECTS)

clean:
	rm -rf $(TARGET) $(OBJECTS)
