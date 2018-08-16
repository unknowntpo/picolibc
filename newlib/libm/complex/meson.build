dsrc_complex = [
  'cabs.c',
  'cacos.c',
  'cacosh.c',
  'carg.c',
  'casin.c',
  'casinh.c',
  'catan.c',
  'catanh.c',
  'ccos.c',
  'ccosh.c',
  'cephes_subr.c',
  'cexp.c',
  'cimag.c',
  'clog.c',
  'clog10.c',
  'conj.c',
  'cpow.c',
  'cproj.c',
  'creal.c',
  'csin.c',
  'csinh.c',
  'csqrt.c',
  'ctan.c',
  'ctanh.c',
]

fsrc_complex = [
  'cabsf.c',
  'casinf.c',
  'ccosf.c',
  'cimagf.c',
  'cprojf.c',
  'csqrtf.c',
  'cacosf.c',
  'casinhf.c',
  'ccoshf.c',
  'clogf.c',
  'clog10f.c',
  'crealf.c',
  'ctanf.c',
  'cacoshf.c',
  'catanf.c',
  'cephes_subrf.c',
  'conjf.c',
  'csinf.c',
  'ctanhf.c',
  'cargf.c',
  'catanhf.c',
  'cexpf.c',
  'cpowf.c',
  'csinhf.c',
]

lsrc_complex = [
  'cabsl.c',
  'creall.c',
  'cimagl.c',
  'ccoshl.c',
  'cacoshl.c',
  'clogl.c',
  'csqrtl.c',
  'cargl.c',
  'cprojl.c',
  'cexpl.c',
  'cephes_subrl.c',
  'cacosl.c',
  'ccosl.c',
  'casinl.c',
  'catanhl.c',
  'conjl.c',
  'cpowl.c',
  'ctanhl.c',
  'ctanl.c',
  'casinhl.c',
  'csinhl.c',
  'csinl.c',
  'catanl.c',
]

srcs_complex = dsrc_complex + fsrc_complex

hdrs_complex = [
    'cephes_subrf.h',
    'cephes_subr.h',
    'cephes_subrl.h',
]
foreach target : targets
	value = get_variable('target_' + target)
	set_variable('lib_complex' + target,
		static_library('complex' + target,
			srcs_complex,
			pic: false,
			include_directories: inc,
			c_args: value[1]))
endforeach