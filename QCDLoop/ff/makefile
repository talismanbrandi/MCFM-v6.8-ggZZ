FC = gfortran
FFLAGS 	= -g 
HERE = $(PWD)
INCDIR = $(HERE)/../Include/
LIBRARY	      = libff.a


# -----------------------------------------------------------------------------
# Specify the object files. 

OBJS	      = \
		ffxc0.o \
		ffxd0.o \
		ffxd0p.o \
		ffxd0i.o \
		ffinit_mine.o \
		ffcc0p.o \
		ffxc0p.o \
		ffcel2.o \
		ffcel3.o \
		ffxc0i.o \
		ffdel2.o \
		ffdel3.o \
		ffdel4.o \
		ffdcc0.o \
		ffxd0h.o \
		ffcxs4.o \
		ffxdbd.o \
		ffcli2.o \
		ffxli2.o \
		ffdxc0.o \
		ffxxyz.o \
		ffcxyz.o \
		fftran.o \
		ff2dl2.o \
		ffcrr.o \
		ffcxs3.o \
		ffdcxs.o \
		ffcxr.o \
		ffabcd.o 


$(LIBRARY):	$(OBJS) 
		ar cru $(LIBRARY) $(OBJS) 
		ranlib $(LIBRARY)
 

.f.o:	
		$(FC) $(F77FLAGS) -I $(INCDIR) -c $*.f


# -----------------------------------------------------------------------------



all:		$(LIBRARY)


# -----------------------------------------------------------------------------

PRJS =      $(OBJS:.o=.f) 
PRJSF =      $(OBJS:.o=.f) 

clean:
	- rm -f *.o *.s *.prj *.a *~ core

# -----------------------------------------------------------------------------

# DO NOT DELETE


