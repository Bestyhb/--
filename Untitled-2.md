| Unbuntu builtin | |
|------------|----|
| job_spec [&] |        |                                                               
| (( expression )) |        |                                                           
| . filename [arguments]                                                              
| :                                                                                   
| [ arg... ]                                                                          
| [[ expression ]]                                                                    
| alias | 别名 | [-p][name[=value]...] | 
| bg [job_spec ...]                                                                   
| bind [-lpsvPSVX] [-m keymap] [-f filename] [-q name] [-u name] [-r keyseq] [-x ke>  
| break [n]                                                                           
| builtin [shell-builtin [arg ...]]                                                   
| caller [expr]                                                                       
| case WORD in [PATTERN [| PATTERN]...) COMMANDS ;;]... esac                          
| cd [-L|[-P [-e]] [-@]] [dir]                                                        
| command [-pVv] command [arg ...]                                                    
| compgen [-abcdefgjksuv] [-o option] [-A action] [-G globpat] [-W wordlist]  [-F f>  
| complete [-abcdefgjksuv] [-pr] [-DE] [-o option] [-A action] [-G globpat] [-W wor>  
| compopt [-o|+o option] [-DE] [name ...]                                             
| continue [n]                                                                        
| coproc [NAME] command [redirections]                                                
| declare [-aAfFgilnrtux] [-p] [name[=value] ...]                                     
| dirs [-clpv] [+N] [-N]                                                              
| disown [-h] [-ar] [jobspec ... | pid ...]                                           
| echo [-neE] [arg ...]                                                               
| enable [-a] [-dnps] [-f filename] [name ...]                                        
| eval [arg ...]                                                                      
| exec [-cl] [-a name] [command [arguments ...]] [redirection ...]                    
| exit [n]                                                                            
| export [-fn] [name[=value] ...] or export -p                                        
| false                                                                               
| fc [-e ename] [-lnr] [first] [last] or fc -s [pat=rep] [command]                    
| fg [job_spec]                                                                       
| for NAME [in WORDS ... ] ; do COMMANDS; done                                        
| for (( exp1; exp2; exp3 )); do COMMANDS; done                                       
| function name { COMMANDS ; } or name () { COMMANDS ; }                              
| getopts optstring name [arg]                                                        
| hash [-lr] [-p pathname] [-dt] [name ...]                                           
| help [-dms] [pattern ...]                                                           
| history [-c] [-d offset] [n] or history -anrw [filename] or history -ps arg [arg>
| if COMMANDS; then COMMANDS; [ elif COMMANDS; then COMMANDS; ]... [ else COMMANDS>
| jobs [-lnprs] [jobspec ...] or jobs -x command [args]
| kill [-s sigspec | -n signum | -sigspec] pid | jobspec ... or kill -l [sigspec]
| let arg [arg ...]
| local [option] name[=value] ...
| logout [n]
| mapfile [-d delim] [-n count] [-O origin] [-s count] [-t] [-u fd] [-C callback] >
| popd [-n] [+N | -N]
| printf [-v var] format [arguments]
| pushd [-n] [+N | -N | dir]
| pwd [-LP]
| read [-ers] [-a array] [-d delim] [-i text] [-n nchars] [-N nchars] [-p prompt] >
| readarray [-n count] [-O origin] [-s count] [-t] [-u fd] [-C callback] [-c quant>
| readonly [-aAf] [name[=value] ...] or readonly -p
| return [n]
| select NAME [in WORDS ... ;] do COMMANDS; done
| set [-abefhkmnptuvxBCHP] [-o option-name] [--] [arg ...]
| shift [n]
| shopt [-pqsu] [-o] [optname ...]
| source filename [arguments]
| suspend [-f]
| test [expr]
| time [-p] pipeline
| times
| trap [-lp] [[arg] signal_spec ...]
| true
| type [-afptP] name [name ...]
| typeset [-aAfFgilnrtux] [-p] name[=value] ...
| ulimit [-SHabcdefiklmnpqrstuvxPT] [limit]
| umask [-p] [-S] [mode]
| unalias [-a] name [name ...]
| unset [-f] [-v] [-n] [name ...]
| until COMMANDS; do COMMANDS; done
| variables - Names and meanings of some shell variables
| wait [-n] [id ...]
| while COMMANDS; do COMMANDS; done
| { COMMANDS ; }
