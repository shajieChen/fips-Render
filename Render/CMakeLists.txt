#
# project: fips-glad\
#  
fips_begin_lib(Render) 
	
	fips_files(
		camera.h
		defs.h
		gl.cpp
		gl.h
		intersect.h
		io.h
		log.h
		math.h
		matrix.h
		util.h
		vector.h
	) 
	
	
fips_end_lib(Render)
if (FIPS_CLANG)
    set_target_properties(Render PROPERTIES COMPILE_FLAGS "-Wno-shift-negative-value")
endif()
