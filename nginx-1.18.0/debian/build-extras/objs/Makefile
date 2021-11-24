
CC =	cc
CFLAGS =  -g -O2 -ffile-prefix-map=/root/ngx/nginx-1.18.0=. -fstack-protector-strong -Wformat -Werror=format-security -g -O2 -ffile-prefix-map=/root/ngx/nginx-1.18.0=. -fstack-protector-strong -Wformat -Werror=format-security -fPIC -Wdate-time -D_FORTIFY_SOURCE=2 -DNDK_SET_VAR
CPP =	
LINK =	$(CC)

NGX_PERL_CFLAGS = -g -O2 -ffile-prefix-map=/root/ngx/nginx-1.18.0=. -fstack-protector-strong -Wformat -Werror=format-security -g -O2 -ffile-prefix-map=/root/ngx/nginx-1.18.0=. -fstack-protector-strong -Wformat -Werror=format-security -fPIC -Wdate-time -D_FORTIFY_SOURCE=2 -DNDK_SET_VAR -D_REENTRANT -D_GNU_SOURCE -DDEBIAN -fwrapv -fno-strict-aliasing -pipe -I/usr/local/include -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64 -I/usr/lib/x86_64-linux-gnu/perl/5.32/CORE
NGX_PM_CFLAGS = -D_REENTRANT -D_GNU_SOURCE -DDEBIAN -fwrapv -fno-strict-aliasing -pipe -I/usr/local/include -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64 -I/usr/lib/x86_64-linux-gnu/perl/5.32/CORE
NGX_PM_LDFLAGS = -shared -L/usr/local/lib -fstack-protector-strong

ALL_INCS = -I src/core \
	-I src/event \
	-I src/event/modules \
	-I src/os/unix \
	-I src/http/modules/perl \
	-I /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module \
	-I /root/ngx/nginx-1.18.0/debian/modules/http-ndk/objs \
	-I objs/addon/ndk \
	-I /root/ngx/nginx-1.18.0/debian/modules/http-ndk/src \
	-I /root/ngx/nginx-1.18.0/debian/modules/http-ndk/objs \
	-I objs/addon/ndk \
	-I /root/ngx/nginx-1.18.0/debian/modules/nchan/src \
	-I /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/api \
	-I /usr/include/luajit-2.1 \
	-I /root/ngx/nginx-1.18.0/debian/modules/rtmp \
	-I /usr/include/libxml2 \
	-I objs \
	-I src/http \
	-I src/http/modules \
	-I src/http/v2 \
	-I /root/ngx/nginx-1.18.0/debian/modules/http-ndk/src \
	-I src/mail \
	-I src/stream


CORE_DEPS = src/core/nginx.h \
	src/core/ngx_config.h \
	src/core/ngx_core.h \
	src/core/ngx_log.h \
	src/core/ngx_palloc.h \
	src/core/ngx_array.h \
	src/core/ngx_list.h \
	src/core/ngx_hash.h \
	src/core/ngx_buf.h \
	src/core/ngx_queue.h \
	src/core/ngx_string.h \
	src/core/ngx_parse.h \
	src/core/ngx_parse_time.h \
	src/core/ngx_inet.h \
	src/core/ngx_file.h \
	src/core/ngx_crc.h \
	src/core/ngx_crc32.h \
	src/core/ngx_murmurhash.h \
	src/core/ngx_md5.h \
	src/core/ngx_sha1.h \
	src/core/ngx_rbtree.h \
	src/core/ngx_radix_tree.h \
	src/core/ngx_rwlock.h \
	src/core/ngx_slab.h \
	src/core/ngx_times.h \
	src/core/ngx_shmtx.h \
	src/core/ngx_connection.h \
	src/core/ngx_cycle.h \
	src/core/ngx_conf_file.h \
	src/core/ngx_module.h \
	src/core/ngx_resolver.h \
	src/core/ngx_open_file_cache.h \
	src/core/ngx_crypt.h \
	src/core/ngx_proxy_protocol.h \
	src/core/ngx_syslog.h \
	src/event/ngx_event.h \
	src/event/ngx_event_timer.h \
	src/event/ngx_event_posted.h \
	src/event/ngx_event_connect.h \
	src/event/ngx_event_pipe.h \
	src/os/unix/ngx_time.h \
	src/os/unix/ngx_errno.h \
	src/os/unix/ngx_alloc.h \
	src/os/unix/ngx_files.h \
	src/os/unix/ngx_channel.h \
	src/os/unix/ngx_shmem.h \
	src/os/unix/ngx_process.h \
	src/os/unix/ngx_setaffinity.h \
	src/os/unix/ngx_setproctitle.h \
	src/os/unix/ngx_atomic.h \
	src/os/unix/ngx_gcc_atomic_x86.h \
	src/os/unix/ngx_thread.h \
	src/os/unix/ngx_socket.h \
	src/os/unix/ngx_os.h \
	src/os/unix/ngx_user.h \
	src/os/unix/ngx_dlopen.h \
	src/os/unix/ngx_process_cycle.h \
	src/os/unix/ngx_linux_config.h \
	src/os/unix/ngx_linux.h \
	src/core/ngx_thread_pool.h \
	src/event/ngx_event_openssl.h \
	src/core/ngx_regex.h \
	objs/ngx_auto_config.h


CORE_INCS = -I src/core \
	-I src/event \
	-I src/event/modules \
	-I src/os/unix \
	-I src/http/modules/perl \
	-I /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module \
	-I /root/ngx/nginx-1.18.0/debian/modules/http-ndk/objs \
	-I objs/addon/ndk \
	-I /root/ngx/nginx-1.18.0/debian/modules/http-ndk/src \
	-I /root/ngx/nginx-1.18.0/debian/modules/http-ndk/objs \
	-I objs/addon/ndk \
	-I /root/ngx/nginx-1.18.0/debian/modules/nchan/src \
	-I /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/api \
	-I /usr/include/luajit-2.1 \
	-I /root/ngx/nginx-1.18.0/debian/modules/rtmp \
	-I /usr/include/libxml2 \
	-I objs


HTTP_DEPS = src/http/ngx_http.h \
	src/http/ngx_http_request.h \
	src/http/ngx_http_config.h \
	src/http/ngx_http_core_module.h \
	src/http/ngx_http_cache.h \
	src/http/ngx_http_variables.h \
	src/http/ngx_http_script.h \
	src/http/ngx_http_upstream.h \
	src/http/ngx_http_upstream_round_robin.h \
	src/http/modules/ngx_http_ssi_filter_module.h \
	src/http/v2/ngx_http_v2.h \
	src/http/v2/ngx_http_v2_module.h \
	src/http/modules/ngx_http_ssl_module.h


HTTP_INCS = -I src/http \
	-I src/http/modules \
	-I src/http/v2 \
	-I /root/ngx/nginx-1.18.0/debian/modules/http-ndk/src


MAIL_DEPS = src/mail/ngx_mail.h \
	src/mail/ngx_mail_ssl_module.h \
	src/mail/ngx_mail_pop3_module.h \
	src/mail/ngx_mail_imap_module.h \
	src/mail/ngx_mail_smtp_module.h


MAIL_INCS = -I src/mail


STREAM_DEPS = src/stream/ngx_stream.h \
	src/stream/ngx_stream_variables.h \
	src/stream/ngx_stream_script.h \
	src/stream/ngx_stream_upstream.h \
	src/stream/ngx_stream_upstream_round_robin.h \
	src/stream/ngx_stream_ssl_module.h


STREAM_INCS = -I src/stream


ADDON_DEPS = $(CORE_DEPS)  src/http/modules/perl/ngx_http_perl_module.h                                                                  /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_amf.h                               /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_bandwidth.h                         /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_cmd_module.h                        /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_codec_module.h                      /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_eval.h                              /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp.h                                   /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_version.h                           /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_live_module.h                       /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_netcall_module.h                    /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_play_module.h                       /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_record_module.h                     /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_relay_module.h                      /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_streams.h                           /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_bitop.h                             /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_proxy_protocol.h                    /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/hls/ngx_rtmp_mpegts.h                        /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/dash/ngx_rtmp_mp4.h                                                                                                    /root/ngx/nginx-1.18.0/debian/modules/http-headers-more-filter/src/ddebug.h                                                 /root/ngx/nginx-1.18.0/debian/modules/http-headers-more-filter/src/ngx_http_headers_more_filter_module.h                    /root/ngx/nginx-1.18.0/debian/modules/http-headers-more-filter/src/ngx_http_headers_more_headers_in.h                       /root/ngx/nginx-1.18.0/debian/modules/http-headers-more-filter/src/ngx_http_headers_more_headers_out.h                      /root/ngx/nginx-1.18.0/debian/modules/http-headers-more-filter/src/ngx_http_headers_more_headers_in.h                       /root/ngx/nginx-1.18.0/debian/modules/http-headers-more-filter/src/ngx_http_headers_more_util.h                              /root/ngx/nginx-1.18.0/debian/modules/http-ndk/src/ndk.h                                                                          /root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ddebug.h                                                 /root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_module.h                                   /root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_handler.h                                  /root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_util.h                                     /root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_sleep.h                                    /root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_filter.h                                   /root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_var.h                                      /root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_location.h                                 /root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_echo.h                                     /root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_request_info.h                             /root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_subrequest.h                               /root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_foreach.h                                   /root/ngx/nginx-1.18.0/debian/modules/http-fancyindex/template.h              /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ddebug.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_script.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_log.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_subrequest.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ndk.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_control.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_time.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_string.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_misc.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_variable.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_output.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_headers.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_uri.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_req_body.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_args.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ctx.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_regex.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_common.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_directive.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_headers_out.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_headers_in.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_consts.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_exception.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_util.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_cache.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_contentby.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_rewriteby.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_accessby.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_setby.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_capturefilter.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_clfactory.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_pcrefix.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_headerfilterby.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_shdict.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_socket_tcp.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/api/ngx_http_lua_api.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_logby.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_sleep.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_semaphore.h            /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_coroutine.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_bodyfilterby.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_initby.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_initworkerby.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_socket_udp.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_req_method.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_phase.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_probe.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_uthread.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_timer.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_config.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_worker.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ssl_certby.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_lex.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_balancer.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ssl_session_storeby.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ssl_session_fetchby.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ssl.h             /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_log_ringbuf.h                                                                               /root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_amf.h                               /root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_bandwidth.h                         /root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_cmd_module.h                        /root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_codec_module.h                      /root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_eval.h                              /root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp.h                                   /root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_version.h                           /root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_live_module.h                       /root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_netcall_module.h                    /root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_play_module.h                       /root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_record_module.h                     /root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_relay_module.h                      /root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_streams.h                           /root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_bitop.h                             /root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_proxy_protocol.h                    /root/ngx/nginx-1.18.0/debian/modules/rtmp/hls/ngx_rtmp_mpegts.h                        /root/ngx/nginx-1.18.0/debian/modules/rtmp/dash/ngx_rtmp_mp4.h                           $(HTTP_DEPS) $(MAIL_DEPS) $(STREAM_DEPS)


build:	binary modules manpage

binary:	objs/nginx

objs/nginx:	objs/src/core/nginx.o \
	objs/src/core/ngx_log.o \
	objs/src/core/ngx_palloc.o \
	objs/src/core/ngx_array.o \
	objs/src/core/ngx_list.o \
	objs/src/core/ngx_hash.o \
	objs/src/core/ngx_buf.o \
	objs/src/core/ngx_queue.o \
	objs/src/core/ngx_output_chain.o \
	objs/src/core/ngx_string.o \
	objs/src/core/ngx_parse.o \
	objs/src/core/ngx_parse_time.o \
	objs/src/core/ngx_inet.o \
	objs/src/core/ngx_file.o \
	objs/src/core/ngx_crc32.o \
	objs/src/core/ngx_murmurhash.o \
	objs/src/core/ngx_md5.o \
	objs/src/core/ngx_sha1.o \
	objs/src/core/ngx_rbtree.o \
	objs/src/core/ngx_radix_tree.o \
	objs/src/core/ngx_slab.o \
	objs/src/core/ngx_times.o \
	objs/src/core/ngx_shmtx.o \
	objs/src/core/ngx_connection.o \
	objs/src/core/ngx_cycle.o \
	objs/src/core/ngx_spinlock.o \
	objs/src/core/ngx_rwlock.o \
	objs/src/core/ngx_cpuinfo.o \
	objs/src/core/ngx_conf_file.o \
	objs/src/core/ngx_module.o \
	objs/src/core/ngx_resolver.o \
	objs/src/core/ngx_open_file_cache.o \
	objs/src/core/ngx_crypt.o \
	objs/src/core/ngx_proxy_protocol.o \
	objs/src/core/ngx_syslog.o \
	objs/src/event/ngx_event.o \
	objs/src/event/ngx_event_timer.o \
	objs/src/event/ngx_event_posted.o \
	objs/src/event/ngx_event_accept.o \
	objs/src/event/ngx_event_udp.o \
	objs/src/event/ngx_event_connect.o \
	objs/src/event/ngx_event_pipe.o \
	objs/src/os/unix/ngx_time.o \
	objs/src/os/unix/ngx_errno.o \
	objs/src/os/unix/ngx_alloc.o \
	objs/src/os/unix/ngx_files.o \
	objs/src/os/unix/ngx_socket.o \
	objs/src/os/unix/ngx_recv.o \
	objs/src/os/unix/ngx_readv_chain.o \
	objs/src/os/unix/ngx_udp_recv.o \
	objs/src/os/unix/ngx_send.o \
	objs/src/os/unix/ngx_writev_chain.o \
	objs/src/os/unix/ngx_udp_send.o \
	objs/src/os/unix/ngx_udp_sendmsg_chain.o \
	objs/src/os/unix/ngx_channel.o \
	objs/src/os/unix/ngx_shmem.o \
	objs/src/os/unix/ngx_process.o \
	objs/src/os/unix/ngx_daemon.o \
	objs/src/os/unix/ngx_setaffinity.o \
	objs/src/os/unix/ngx_setproctitle.o \
	objs/src/os/unix/ngx_posix_init.o \
	objs/src/os/unix/ngx_user.o \
	objs/src/os/unix/ngx_dlopen.o \
	objs/src/os/unix/ngx_process_cycle.o \
	objs/src/os/unix/ngx_linux_init.o \
	objs/src/event/modules/ngx_epoll_module.o \
	objs/src/os/unix/ngx_linux_sendfile_chain.o \
	objs/src/core/ngx_thread_pool.o \
	objs/src/os/unix/ngx_thread_cond.o \
	objs/src/os/unix/ngx_thread_mutex.o \
	objs/src/os/unix/ngx_thread_id.o \
	objs/src/event/ngx_event_openssl.o \
	objs/src/event/ngx_event_openssl_stapling.o \
	objs/src/core/ngx_regex.o \
	objs/src/http/ngx_http.o \
	objs/src/http/ngx_http_core_module.o \
	objs/src/http/ngx_http_special_response.o \
	objs/src/http/ngx_http_request.o \
	objs/src/http/ngx_http_parse.o \
	objs/src/http/modules/ngx_http_log_module.o \
	objs/src/http/ngx_http_request_body.o \
	objs/src/http/ngx_http_variables.o \
	objs/src/http/ngx_http_script.o \
	objs/src/http/ngx_http_upstream.o \
	objs/src/http/ngx_http_upstream_round_robin.o \
	objs/src/http/ngx_http_file_cache.o \
	objs/src/http/ngx_http_write_filter_module.o \
	objs/src/http/ngx_http_header_filter_module.o \
	objs/src/http/modules/ngx_http_chunked_filter_module.o \
	objs/src/http/v2/ngx_http_v2_filter_module.o \
	objs/src/http/modules/ngx_http_range_filter_module.o \
	objs/src/http/modules/ngx_http_gzip_filter_module.o \
	objs/src/http/ngx_http_postpone_filter_module.o \
	objs/src/http/modules/ngx_http_ssi_filter_module.o \
	objs/src/http/modules/ngx_http_charset_filter_module.o \
	objs/src/http/modules/ngx_http_sub_filter_module.o \
	objs/src/http/modules/ngx_http_addition_filter_module.o \
	objs/src/http/modules/ngx_http_gunzip_filter_module.o \
	objs/src/http/modules/ngx_http_userid_filter_module.o \
	objs/src/http/modules/ngx_http_headers_filter_module.o \
	objs/src/http/ngx_http_copy_filter_module.o \
	objs/src/http/modules/ngx_http_not_modified_filter_module.o \
	objs/src/http/modules/ngx_http_slice_filter_module.o \
	objs/src/http/v2/ngx_http_v2.o \
	objs/src/http/v2/ngx_http_v2_table.o \
	objs/src/http/v2/ngx_http_v2_encode.o \
	objs/src/http/v2/ngx_http_v2_huff_decode.o \
	objs/src/http/v2/ngx_http_v2_huff_encode.o \
	objs/src/http/v2/ngx_http_v2_module.o \
	objs/src/http/modules/ngx_http_static_module.o \
	objs/src/http/modules/ngx_http_gzip_static_module.o \
	objs/src/http/modules/ngx_http_dav_module.o \
	objs/src/http/modules/ngx_http_autoindex_module.o \
	objs/src/http/modules/ngx_http_index_module.o \
	objs/src/http/modules/ngx_http_random_index_module.o \
	objs/src/http/modules/ngx_http_mirror_module.o \
	objs/src/http/modules/ngx_http_try_files_module.o \
	objs/src/http/modules/ngx_http_auth_request_module.o \
	objs/src/http/modules/ngx_http_auth_basic_module.o \
	objs/src/http/modules/ngx_http_access_module.o \
	objs/src/http/modules/ngx_http_limit_conn_module.o \
	objs/src/http/modules/ngx_http_limit_req_module.o \
	objs/src/http/modules/ngx_http_realip_module.o \
	objs/src/http/modules/ngx_http_geo_module.o \
	objs/src/http/modules/ngx_http_map_module.o \
	objs/src/http/modules/ngx_http_split_clients_module.o \
	objs/src/http/modules/ngx_http_referer_module.o \
	objs/src/http/modules/ngx_http_rewrite_module.o \
	objs/src/http/modules/ngx_http_ssl_module.o \
	objs/src/http/modules/ngx_http_proxy_module.o \
	objs/src/http/modules/ngx_http_fastcgi_module.o \
	objs/src/http/modules/ngx_http_uwsgi_module.o \
	objs/src/http/modules/ngx_http_scgi_module.o \
	objs/src/http/modules/ngx_http_grpc_module.o \
	objs/src/http/modules/ngx_http_memcached_module.o \
	objs/src/http/modules/ngx_http_empty_gif_module.o \
	objs/src/http/modules/ngx_http_browser_module.o \
	objs/src/http/modules/ngx_http_secure_link_module.o \
	objs/src/http/modules/ngx_http_flv_module.o \
	objs/src/http/modules/ngx_http_mp4_module.o \
	objs/src/http/modules/ngx_http_upstream_hash_module.o \
	objs/src/http/modules/ngx_http_upstream_ip_hash_module.o \
	objs/src/http/modules/ngx_http_upstream_least_conn_module.o \
	objs/src/http/modules/ngx_http_upstream_random_module.o \
	objs/src/http/modules/ngx_http_upstream_keepalive_module.o \
	objs/src/http/modules/ngx_http_upstream_zone_module.o \
	objs/src/http/modules/ngx_http_stub_status_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_init.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_handshake.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_handler.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_amf.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_send.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_shared.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_eval.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_receive.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_core_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_cmd_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_codec_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_access_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_record_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_live_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_play_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_flv_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_mp4_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_netcall_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_relay_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_bandwidth.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_exec_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_auto_push_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_notify_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_log_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_limit_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_bitop.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_proxy_protocol.o \
	objs/addon/hls/ngx_rtmp_hls_module.o \
	objs/addon/dash/ngx_rtmp_dash_module.o \
	objs/addon/hls/ngx_rtmp_mpegts.o \
	objs/addon/dash/ngx_rtmp_mp4.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_stat_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_control_module.o \
	objs/ngx_modules.o

	$(LINK) -o objs/nginx \
	objs/src/core/nginx.o \
	objs/src/core/ngx_log.o \
	objs/src/core/ngx_palloc.o \
	objs/src/core/ngx_array.o \
	objs/src/core/ngx_list.o \
	objs/src/core/ngx_hash.o \
	objs/src/core/ngx_buf.o \
	objs/src/core/ngx_queue.o \
	objs/src/core/ngx_output_chain.o \
	objs/src/core/ngx_string.o \
	objs/src/core/ngx_parse.o \
	objs/src/core/ngx_parse_time.o \
	objs/src/core/ngx_inet.o \
	objs/src/core/ngx_file.o \
	objs/src/core/ngx_crc32.o \
	objs/src/core/ngx_murmurhash.o \
	objs/src/core/ngx_md5.o \
	objs/src/core/ngx_sha1.o \
	objs/src/core/ngx_rbtree.o \
	objs/src/core/ngx_radix_tree.o \
	objs/src/core/ngx_slab.o \
	objs/src/core/ngx_times.o \
	objs/src/core/ngx_shmtx.o \
	objs/src/core/ngx_connection.o \
	objs/src/core/ngx_cycle.o \
	objs/src/core/ngx_spinlock.o \
	objs/src/core/ngx_rwlock.o \
	objs/src/core/ngx_cpuinfo.o \
	objs/src/core/ngx_conf_file.o \
	objs/src/core/ngx_module.o \
	objs/src/core/ngx_resolver.o \
	objs/src/core/ngx_open_file_cache.o \
	objs/src/core/ngx_crypt.o \
	objs/src/core/ngx_proxy_protocol.o \
	objs/src/core/ngx_syslog.o \
	objs/src/event/ngx_event.o \
	objs/src/event/ngx_event_timer.o \
	objs/src/event/ngx_event_posted.o \
	objs/src/event/ngx_event_accept.o \
	objs/src/event/ngx_event_udp.o \
	objs/src/event/ngx_event_connect.o \
	objs/src/event/ngx_event_pipe.o \
	objs/src/os/unix/ngx_time.o \
	objs/src/os/unix/ngx_errno.o \
	objs/src/os/unix/ngx_alloc.o \
	objs/src/os/unix/ngx_files.o \
	objs/src/os/unix/ngx_socket.o \
	objs/src/os/unix/ngx_recv.o \
	objs/src/os/unix/ngx_readv_chain.o \
	objs/src/os/unix/ngx_udp_recv.o \
	objs/src/os/unix/ngx_send.o \
	objs/src/os/unix/ngx_writev_chain.o \
	objs/src/os/unix/ngx_udp_send.o \
	objs/src/os/unix/ngx_udp_sendmsg_chain.o \
	objs/src/os/unix/ngx_channel.o \
	objs/src/os/unix/ngx_shmem.o \
	objs/src/os/unix/ngx_process.o \
	objs/src/os/unix/ngx_daemon.o \
	objs/src/os/unix/ngx_setaffinity.o \
	objs/src/os/unix/ngx_setproctitle.o \
	objs/src/os/unix/ngx_posix_init.o \
	objs/src/os/unix/ngx_user.o \
	objs/src/os/unix/ngx_dlopen.o \
	objs/src/os/unix/ngx_process_cycle.o \
	objs/src/os/unix/ngx_linux_init.o \
	objs/src/event/modules/ngx_epoll_module.o \
	objs/src/os/unix/ngx_linux_sendfile_chain.o \
	objs/src/core/ngx_thread_pool.o \
	objs/src/os/unix/ngx_thread_cond.o \
	objs/src/os/unix/ngx_thread_mutex.o \
	objs/src/os/unix/ngx_thread_id.o \
	objs/src/event/ngx_event_openssl.o \
	objs/src/event/ngx_event_openssl_stapling.o \
	objs/src/core/ngx_regex.o \
	objs/src/http/ngx_http.o \
	objs/src/http/ngx_http_core_module.o \
	objs/src/http/ngx_http_special_response.o \
	objs/src/http/ngx_http_request.o \
	objs/src/http/ngx_http_parse.o \
	objs/src/http/modules/ngx_http_log_module.o \
	objs/src/http/ngx_http_request_body.o \
	objs/src/http/ngx_http_variables.o \
	objs/src/http/ngx_http_script.o \
	objs/src/http/ngx_http_upstream.o \
	objs/src/http/ngx_http_upstream_round_robin.o \
	objs/src/http/ngx_http_file_cache.o \
	objs/src/http/ngx_http_write_filter_module.o \
	objs/src/http/ngx_http_header_filter_module.o \
	objs/src/http/modules/ngx_http_chunked_filter_module.o \
	objs/src/http/v2/ngx_http_v2_filter_module.o \
	objs/src/http/modules/ngx_http_range_filter_module.o \
	objs/src/http/modules/ngx_http_gzip_filter_module.o \
	objs/src/http/ngx_http_postpone_filter_module.o \
	objs/src/http/modules/ngx_http_ssi_filter_module.o \
	objs/src/http/modules/ngx_http_charset_filter_module.o \
	objs/src/http/modules/ngx_http_sub_filter_module.o \
	objs/src/http/modules/ngx_http_addition_filter_module.o \
	objs/src/http/modules/ngx_http_gunzip_filter_module.o \
	objs/src/http/modules/ngx_http_userid_filter_module.o \
	objs/src/http/modules/ngx_http_headers_filter_module.o \
	objs/src/http/ngx_http_copy_filter_module.o \
	objs/src/http/modules/ngx_http_not_modified_filter_module.o \
	objs/src/http/modules/ngx_http_slice_filter_module.o \
	objs/src/http/v2/ngx_http_v2.o \
	objs/src/http/v2/ngx_http_v2_table.o \
	objs/src/http/v2/ngx_http_v2_encode.o \
	objs/src/http/v2/ngx_http_v2_huff_decode.o \
	objs/src/http/v2/ngx_http_v2_huff_encode.o \
	objs/src/http/v2/ngx_http_v2_module.o \
	objs/src/http/modules/ngx_http_static_module.o \
	objs/src/http/modules/ngx_http_gzip_static_module.o \
	objs/src/http/modules/ngx_http_dav_module.o \
	objs/src/http/modules/ngx_http_autoindex_module.o \
	objs/src/http/modules/ngx_http_index_module.o \
	objs/src/http/modules/ngx_http_random_index_module.o \
	objs/src/http/modules/ngx_http_mirror_module.o \
	objs/src/http/modules/ngx_http_try_files_module.o \
	objs/src/http/modules/ngx_http_auth_request_module.o \
	objs/src/http/modules/ngx_http_auth_basic_module.o \
	objs/src/http/modules/ngx_http_access_module.o \
	objs/src/http/modules/ngx_http_limit_conn_module.o \
	objs/src/http/modules/ngx_http_limit_req_module.o \
	objs/src/http/modules/ngx_http_realip_module.o \
	objs/src/http/modules/ngx_http_geo_module.o \
	objs/src/http/modules/ngx_http_map_module.o \
	objs/src/http/modules/ngx_http_split_clients_module.o \
	objs/src/http/modules/ngx_http_referer_module.o \
	objs/src/http/modules/ngx_http_rewrite_module.o \
	objs/src/http/modules/ngx_http_ssl_module.o \
	objs/src/http/modules/ngx_http_proxy_module.o \
	objs/src/http/modules/ngx_http_fastcgi_module.o \
	objs/src/http/modules/ngx_http_uwsgi_module.o \
	objs/src/http/modules/ngx_http_scgi_module.o \
	objs/src/http/modules/ngx_http_grpc_module.o \
	objs/src/http/modules/ngx_http_memcached_module.o \
	objs/src/http/modules/ngx_http_empty_gif_module.o \
	objs/src/http/modules/ngx_http_browser_module.o \
	objs/src/http/modules/ngx_http_secure_link_module.o \
	objs/src/http/modules/ngx_http_flv_module.o \
	objs/src/http/modules/ngx_http_mp4_module.o \
	objs/src/http/modules/ngx_http_upstream_hash_module.o \
	objs/src/http/modules/ngx_http_upstream_ip_hash_module.o \
	objs/src/http/modules/ngx_http_upstream_least_conn_module.o \
	objs/src/http/modules/ngx_http_upstream_random_module.o \
	objs/src/http/modules/ngx_http_upstream_keepalive_module.o \
	objs/src/http/modules/ngx_http_upstream_zone_module.o \
	objs/src/http/modules/ngx_http_stub_status_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_init.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_handshake.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_handler.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_amf.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_send.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_shared.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_eval.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_receive.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_core_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_cmd_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_codec_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_access_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_record_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_live_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_play_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_flv_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_mp4_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_netcall_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_relay_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_bandwidth.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_exec_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_auto_push_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_notify_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_log_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_limit_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_bitop.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_proxy_protocol.o \
	objs/addon/hls/ngx_rtmp_hls_module.o \
	objs/addon/dash/ngx_rtmp_dash_module.o \
	objs/addon/hls/ngx_rtmp_mpegts.o \
	objs/addon/dash/ngx_rtmp_mp4.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_stat_module.o \
	objs/addon/nginx-rtmp-module/ngx_rtmp_control_module.o \
	objs/ngx_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC -Wl,-E -ldl -lpthread -lpthread -lcrypt -lpcre -lssl -lcrypto -ldl -lpthread -lz \
	-Wl,-E
	


modules:

objs/ngx_modules.o:	$(CORE_DEPS) \
	objs/ngx_modules.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/ngx_modules.o \
		objs/ngx_modules.c


objs/src/core/nginx.o:	$(CORE_DEPS) \
	src/core/nginx.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/nginx.o \
		src/core/nginx.c


objs/src/core/ngx_log.o:	$(CORE_DEPS) \
	src/core/ngx_log.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_log.o \
		src/core/ngx_log.c


objs/src/core/ngx_palloc.o:	$(CORE_DEPS) \
	src/core/ngx_palloc.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_palloc.o \
		src/core/ngx_palloc.c


objs/src/core/ngx_array.o:	$(CORE_DEPS) \
	src/core/ngx_array.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_array.o \
		src/core/ngx_array.c


objs/src/core/ngx_list.o:	$(CORE_DEPS) \
	src/core/ngx_list.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_list.o \
		src/core/ngx_list.c


objs/src/core/ngx_hash.o:	$(CORE_DEPS) \
	src/core/ngx_hash.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_hash.o \
		src/core/ngx_hash.c


objs/src/core/ngx_buf.o:	$(CORE_DEPS) \
	src/core/ngx_buf.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_buf.o \
		src/core/ngx_buf.c


objs/src/core/ngx_queue.o:	$(CORE_DEPS) \
	src/core/ngx_queue.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_queue.o \
		src/core/ngx_queue.c


objs/src/core/ngx_output_chain.o:	$(CORE_DEPS) \
	src/core/ngx_output_chain.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_output_chain.o \
		src/core/ngx_output_chain.c


objs/src/core/ngx_string.o:	$(CORE_DEPS) \
	src/core/ngx_string.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_string.o \
		src/core/ngx_string.c


objs/src/core/ngx_parse.o:	$(CORE_DEPS) \
	src/core/ngx_parse.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_parse.o \
		src/core/ngx_parse.c


objs/src/core/ngx_parse_time.o:	$(CORE_DEPS) \
	src/core/ngx_parse_time.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_parse_time.o \
		src/core/ngx_parse_time.c


objs/src/core/ngx_inet.o:	$(CORE_DEPS) \
	src/core/ngx_inet.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_inet.o \
		src/core/ngx_inet.c


objs/src/core/ngx_file.o:	$(CORE_DEPS) \
	src/core/ngx_file.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_file.o \
		src/core/ngx_file.c


objs/src/core/ngx_crc32.o:	$(CORE_DEPS) \
	src/core/ngx_crc32.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_crc32.o \
		src/core/ngx_crc32.c


objs/src/core/ngx_murmurhash.o:	$(CORE_DEPS) \
	src/core/ngx_murmurhash.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_murmurhash.o \
		src/core/ngx_murmurhash.c


objs/src/core/ngx_md5.o:	$(CORE_DEPS) \
	src/core/ngx_md5.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_md5.o \
		src/core/ngx_md5.c


objs/src/core/ngx_sha1.o:	$(CORE_DEPS) \
	src/core/ngx_sha1.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_sha1.o \
		src/core/ngx_sha1.c


objs/src/core/ngx_rbtree.o:	$(CORE_DEPS) \
	src/core/ngx_rbtree.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_rbtree.o \
		src/core/ngx_rbtree.c


objs/src/core/ngx_radix_tree.o:	$(CORE_DEPS) \
	src/core/ngx_radix_tree.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_radix_tree.o \
		src/core/ngx_radix_tree.c


objs/src/core/ngx_slab.o:	$(CORE_DEPS) \
	src/core/ngx_slab.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_slab.o \
		src/core/ngx_slab.c


objs/src/core/ngx_times.o:	$(CORE_DEPS) \
	src/core/ngx_times.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_times.o \
		src/core/ngx_times.c


objs/src/core/ngx_shmtx.o:	$(CORE_DEPS) \
	src/core/ngx_shmtx.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_shmtx.o \
		src/core/ngx_shmtx.c


objs/src/core/ngx_connection.o:	$(CORE_DEPS) \
	src/core/ngx_connection.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_connection.o \
		src/core/ngx_connection.c


objs/src/core/ngx_cycle.o:	$(CORE_DEPS) \
	src/core/ngx_cycle.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_cycle.o \
		src/core/ngx_cycle.c


objs/src/core/ngx_spinlock.o:	$(CORE_DEPS) \
	src/core/ngx_spinlock.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_spinlock.o \
		src/core/ngx_spinlock.c


objs/src/core/ngx_rwlock.o:	$(CORE_DEPS) \
	src/core/ngx_rwlock.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_rwlock.o \
		src/core/ngx_rwlock.c


objs/src/core/ngx_cpuinfo.o:	$(CORE_DEPS) \
	src/core/ngx_cpuinfo.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_cpuinfo.o \
		src/core/ngx_cpuinfo.c


objs/src/core/ngx_conf_file.o:	$(CORE_DEPS) \
	src/core/ngx_conf_file.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_conf_file.o \
		src/core/ngx_conf_file.c


objs/src/core/ngx_module.o:	$(CORE_DEPS) \
	src/core/ngx_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_module.o \
		src/core/ngx_module.c


objs/src/core/ngx_resolver.o:	$(CORE_DEPS) \
	src/core/ngx_resolver.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_resolver.o \
		src/core/ngx_resolver.c


objs/src/core/ngx_open_file_cache.o:	$(CORE_DEPS) \
	src/core/ngx_open_file_cache.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_open_file_cache.o \
		src/core/ngx_open_file_cache.c


objs/src/core/ngx_crypt.o:	$(CORE_DEPS) \
	src/core/ngx_crypt.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_crypt.o \
		src/core/ngx_crypt.c


objs/src/core/ngx_proxy_protocol.o:	$(CORE_DEPS) \
	src/core/ngx_proxy_protocol.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_proxy_protocol.o \
		src/core/ngx_proxy_protocol.c


objs/src/core/ngx_syslog.o:	$(CORE_DEPS) \
	src/core/ngx_syslog.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_syslog.o \
		src/core/ngx_syslog.c


objs/src/event/ngx_event.o:	$(CORE_DEPS) \
	src/event/ngx_event.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/event/ngx_event.o \
		src/event/ngx_event.c


objs/src/event/ngx_event_timer.o:	$(CORE_DEPS) \
	src/event/ngx_event_timer.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/event/ngx_event_timer.o \
		src/event/ngx_event_timer.c


objs/src/event/ngx_event_posted.o:	$(CORE_DEPS) \
	src/event/ngx_event_posted.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/event/ngx_event_posted.o \
		src/event/ngx_event_posted.c


objs/src/event/ngx_event_accept.o:	$(CORE_DEPS) \
	src/event/ngx_event_accept.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/event/ngx_event_accept.o \
		src/event/ngx_event_accept.c


objs/src/event/ngx_event_udp.o:	$(CORE_DEPS) \
	src/event/ngx_event_udp.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/event/ngx_event_udp.o \
		src/event/ngx_event_udp.c


objs/src/event/ngx_event_connect.o:	$(CORE_DEPS) \
	src/event/ngx_event_connect.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/event/ngx_event_connect.o \
		src/event/ngx_event_connect.c


objs/src/event/ngx_event_pipe.o:	$(CORE_DEPS) \
	src/event/ngx_event_pipe.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/event/ngx_event_pipe.o \
		src/event/ngx_event_pipe.c


objs/src/os/unix/ngx_time.o:	$(CORE_DEPS) \
	src/os/unix/ngx_time.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_time.o \
		src/os/unix/ngx_time.c


objs/src/os/unix/ngx_errno.o:	$(CORE_DEPS) \
	src/os/unix/ngx_errno.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_errno.o \
		src/os/unix/ngx_errno.c


objs/src/os/unix/ngx_alloc.o:	$(CORE_DEPS) \
	src/os/unix/ngx_alloc.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_alloc.o \
		src/os/unix/ngx_alloc.c


objs/src/os/unix/ngx_files.o:	$(CORE_DEPS) \
	src/os/unix/ngx_files.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_files.o \
		src/os/unix/ngx_files.c


objs/src/os/unix/ngx_socket.o:	$(CORE_DEPS) \
	src/os/unix/ngx_socket.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_socket.o \
		src/os/unix/ngx_socket.c


objs/src/os/unix/ngx_recv.o:	$(CORE_DEPS) \
	src/os/unix/ngx_recv.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_recv.o \
		src/os/unix/ngx_recv.c


objs/src/os/unix/ngx_readv_chain.o:	$(CORE_DEPS) \
	src/os/unix/ngx_readv_chain.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_readv_chain.o \
		src/os/unix/ngx_readv_chain.c


objs/src/os/unix/ngx_udp_recv.o:	$(CORE_DEPS) \
	src/os/unix/ngx_udp_recv.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_udp_recv.o \
		src/os/unix/ngx_udp_recv.c


objs/src/os/unix/ngx_send.o:	$(CORE_DEPS) \
	src/os/unix/ngx_send.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_send.o \
		src/os/unix/ngx_send.c


objs/src/os/unix/ngx_writev_chain.o:	$(CORE_DEPS) \
	src/os/unix/ngx_writev_chain.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_writev_chain.o \
		src/os/unix/ngx_writev_chain.c


objs/src/os/unix/ngx_udp_send.o:	$(CORE_DEPS) \
	src/os/unix/ngx_udp_send.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_udp_send.o \
		src/os/unix/ngx_udp_send.c


objs/src/os/unix/ngx_udp_sendmsg_chain.o:	$(CORE_DEPS) \
	src/os/unix/ngx_udp_sendmsg_chain.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_udp_sendmsg_chain.o \
		src/os/unix/ngx_udp_sendmsg_chain.c


objs/src/os/unix/ngx_channel.o:	$(CORE_DEPS) \
	src/os/unix/ngx_channel.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_channel.o \
		src/os/unix/ngx_channel.c


objs/src/os/unix/ngx_shmem.o:	$(CORE_DEPS) \
	src/os/unix/ngx_shmem.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_shmem.o \
		src/os/unix/ngx_shmem.c


objs/src/os/unix/ngx_process.o:	$(CORE_DEPS) \
	src/os/unix/ngx_process.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_process.o \
		src/os/unix/ngx_process.c


objs/src/os/unix/ngx_daemon.o:	$(CORE_DEPS) \
	src/os/unix/ngx_daemon.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_daemon.o \
		src/os/unix/ngx_daemon.c


objs/src/os/unix/ngx_setaffinity.o:	$(CORE_DEPS) \
	src/os/unix/ngx_setaffinity.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_setaffinity.o \
		src/os/unix/ngx_setaffinity.c


objs/src/os/unix/ngx_setproctitle.o:	$(CORE_DEPS) \
	src/os/unix/ngx_setproctitle.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_setproctitle.o \
		src/os/unix/ngx_setproctitle.c


objs/src/os/unix/ngx_posix_init.o:	$(CORE_DEPS) \
	src/os/unix/ngx_posix_init.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_posix_init.o \
		src/os/unix/ngx_posix_init.c


objs/src/os/unix/ngx_user.o:	$(CORE_DEPS) \
	src/os/unix/ngx_user.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_user.o \
		src/os/unix/ngx_user.c


objs/src/os/unix/ngx_dlopen.o:	$(CORE_DEPS) \
	src/os/unix/ngx_dlopen.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_dlopen.o \
		src/os/unix/ngx_dlopen.c


objs/src/os/unix/ngx_process_cycle.o:	$(CORE_DEPS) \
	src/os/unix/ngx_process_cycle.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_process_cycle.o \
		src/os/unix/ngx_process_cycle.c


objs/src/os/unix/ngx_linux_init.o:	$(CORE_DEPS) \
	src/os/unix/ngx_linux_init.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_linux_init.o \
		src/os/unix/ngx_linux_init.c


objs/src/event/modules/ngx_epoll_module.o:	$(CORE_DEPS) \
	src/event/modules/ngx_epoll_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/event/modules/ngx_epoll_module.o \
		src/event/modules/ngx_epoll_module.c


objs/src/os/unix/ngx_linux_sendfile_chain.o:	$(CORE_DEPS) \
	src/os/unix/ngx_linux_sendfile_chain.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_linux_sendfile_chain.o \
		src/os/unix/ngx_linux_sendfile_chain.c


objs/src/core/ngx_thread_pool.o:	$(CORE_DEPS) \
	src/core/ngx_thread_pool.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_thread_pool.o \
		src/core/ngx_thread_pool.c


objs/src/os/unix/ngx_thread_cond.o:	$(CORE_DEPS) \
	src/os/unix/ngx_thread_cond.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_thread_cond.o \
		src/os/unix/ngx_thread_cond.c


objs/src/os/unix/ngx_thread_mutex.o:	$(CORE_DEPS) \
	src/os/unix/ngx_thread_mutex.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_thread_mutex.o \
		src/os/unix/ngx_thread_mutex.c


objs/src/os/unix/ngx_thread_id.o:	$(CORE_DEPS) \
	src/os/unix/ngx_thread_id.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/os/unix/ngx_thread_id.o \
		src/os/unix/ngx_thread_id.c


objs/src/event/ngx_event_openssl.o:	$(CORE_DEPS) \
	src/event/ngx_event_openssl.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/event/ngx_event_openssl.o \
		src/event/ngx_event_openssl.c


objs/src/event/ngx_event_openssl_stapling.o:	$(CORE_DEPS) \
	src/event/ngx_event_openssl_stapling.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/event/ngx_event_openssl_stapling.o \
		src/event/ngx_event_openssl_stapling.c


objs/src/core/ngx_regex.o:	$(CORE_DEPS) \
	src/core/ngx_regex.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) \
		-o objs/src/core/ngx_regex.o \
		src/core/ngx_regex.c


objs/src/http/ngx_http.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/ngx_http.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/ngx_http.o \
		src/http/ngx_http.c


objs/src/http/ngx_http_core_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/ngx_http_core_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/ngx_http_core_module.o \
		src/http/ngx_http_core_module.c


objs/src/http/ngx_http_special_response.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/ngx_http_special_response.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/ngx_http_special_response.o \
		src/http/ngx_http_special_response.c


objs/src/http/ngx_http_request.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/ngx_http_request.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/ngx_http_request.o \
		src/http/ngx_http_request.c


objs/src/http/ngx_http_parse.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/ngx_http_parse.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/ngx_http_parse.o \
		src/http/ngx_http_parse.c


objs/src/http/modules/ngx_http_log_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_log_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_log_module.o \
		src/http/modules/ngx_http_log_module.c


objs/src/http/ngx_http_request_body.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/ngx_http_request_body.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/ngx_http_request_body.o \
		src/http/ngx_http_request_body.c


objs/src/http/ngx_http_variables.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/ngx_http_variables.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/ngx_http_variables.o \
		src/http/ngx_http_variables.c


objs/src/http/ngx_http_script.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/ngx_http_script.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/ngx_http_script.o \
		src/http/ngx_http_script.c


objs/src/http/ngx_http_upstream.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/ngx_http_upstream.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/ngx_http_upstream.o \
		src/http/ngx_http_upstream.c


objs/src/http/ngx_http_upstream_round_robin.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/ngx_http_upstream_round_robin.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/ngx_http_upstream_round_robin.o \
		src/http/ngx_http_upstream_round_robin.c


objs/src/http/ngx_http_file_cache.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/ngx_http_file_cache.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/ngx_http_file_cache.o \
		src/http/ngx_http_file_cache.c


objs/src/http/ngx_http_write_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/ngx_http_write_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/ngx_http_write_filter_module.o \
		src/http/ngx_http_write_filter_module.c


objs/src/http/ngx_http_header_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/ngx_http_header_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/ngx_http_header_filter_module.o \
		src/http/ngx_http_header_filter_module.c


objs/src/http/modules/ngx_http_chunked_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_chunked_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_chunked_filter_module.o \
		src/http/modules/ngx_http_chunked_filter_module.c


objs/src/http/v2/ngx_http_v2_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/v2/ngx_http_v2_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/v2/ngx_http_v2_filter_module.o \
		src/http/v2/ngx_http_v2_filter_module.c


objs/src/http/modules/ngx_http_range_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_range_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_range_filter_module.o \
		src/http/modules/ngx_http_range_filter_module.c


objs/src/http/modules/ngx_http_gzip_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_gzip_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_gzip_filter_module.o \
		src/http/modules/ngx_http_gzip_filter_module.c


objs/src/http/ngx_http_postpone_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/ngx_http_postpone_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/ngx_http_postpone_filter_module.o \
		src/http/ngx_http_postpone_filter_module.c


objs/src/http/modules/ngx_http_ssi_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_ssi_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_ssi_filter_module.o \
		src/http/modules/ngx_http_ssi_filter_module.c


objs/src/http/modules/ngx_http_charset_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_charset_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_charset_filter_module.o \
		src/http/modules/ngx_http_charset_filter_module.c


objs/src/http/modules/ngx_http_sub_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_sub_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_sub_filter_module.o \
		src/http/modules/ngx_http_sub_filter_module.c


objs/src/http/modules/ngx_http_addition_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_addition_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_addition_filter_module.o \
		src/http/modules/ngx_http_addition_filter_module.c


objs/src/http/modules/ngx_http_gunzip_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_gunzip_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_gunzip_filter_module.o \
		src/http/modules/ngx_http_gunzip_filter_module.c


objs/src/http/modules/ngx_http_userid_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_userid_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_userid_filter_module.o \
		src/http/modules/ngx_http_userid_filter_module.c


objs/src/http/modules/ngx_http_headers_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_headers_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_headers_filter_module.o \
		src/http/modules/ngx_http_headers_filter_module.c


objs/src/http/ngx_http_copy_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/ngx_http_copy_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/ngx_http_copy_filter_module.o \
		src/http/ngx_http_copy_filter_module.c


objs/src/http/modules/ngx_http_not_modified_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_not_modified_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_not_modified_filter_module.o \
		src/http/modules/ngx_http_not_modified_filter_module.c


objs/src/http/modules/ngx_http_slice_filter_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_slice_filter_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_slice_filter_module.o \
		src/http/modules/ngx_http_slice_filter_module.c


objs/src/http/v2/ngx_http_v2.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/v2/ngx_http_v2.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/v2/ngx_http_v2.o \
		src/http/v2/ngx_http_v2.c


objs/src/http/v2/ngx_http_v2_table.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/v2/ngx_http_v2_table.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/v2/ngx_http_v2_table.o \
		src/http/v2/ngx_http_v2_table.c


objs/src/http/v2/ngx_http_v2_encode.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/v2/ngx_http_v2_encode.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/v2/ngx_http_v2_encode.o \
		src/http/v2/ngx_http_v2_encode.c


objs/src/http/v2/ngx_http_v2_huff_decode.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/v2/ngx_http_v2_huff_decode.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/v2/ngx_http_v2_huff_decode.o \
		src/http/v2/ngx_http_v2_huff_decode.c


objs/src/http/v2/ngx_http_v2_huff_encode.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/v2/ngx_http_v2_huff_encode.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/v2/ngx_http_v2_huff_encode.o \
		src/http/v2/ngx_http_v2_huff_encode.c


objs/src/http/v2/ngx_http_v2_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/v2/ngx_http_v2_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/v2/ngx_http_v2_module.o \
		src/http/v2/ngx_http_v2_module.c


objs/src/http/modules/ngx_http_static_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_static_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_static_module.o \
		src/http/modules/ngx_http_static_module.c


objs/src/http/modules/ngx_http_gzip_static_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_gzip_static_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_gzip_static_module.o \
		src/http/modules/ngx_http_gzip_static_module.c


objs/src/http/modules/ngx_http_dav_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_dav_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_dav_module.o \
		src/http/modules/ngx_http_dav_module.c


objs/src/http/modules/ngx_http_autoindex_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_autoindex_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_autoindex_module.o \
		src/http/modules/ngx_http_autoindex_module.c


objs/src/http/modules/ngx_http_index_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_index_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_index_module.o \
		src/http/modules/ngx_http_index_module.c


objs/src/http/modules/ngx_http_random_index_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_random_index_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_random_index_module.o \
		src/http/modules/ngx_http_random_index_module.c


objs/src/http/modules/ngx_http_mirror_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_mirror_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_mirror_module.o \
		src/http/modules/ngx_http_mirror_module.c


objs/src/http/modules/ngx_http_try_files_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_try_files_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_try_files_module.o \
		src/http/modules/ngx_http_try_files_module.c


objs/src/http/modules/ngx_http_auth_request_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_auth_request_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_auth_request_module.o \
		src/http/modules/ngx_http_auth_request_module.c


objs/src/http/modules/ngx_http_auth_basic_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_auth_basic_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_auth_basic_module.o \
		src/http/modules/ngx_http_auth_basic_module.c


objs/src/http/modules/ngx_http_access_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_access_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_access_module.o \
		src/http/modules/ngx_http_access_module.c


objs/src/http/modules/ngx_http_limit_conn_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_limit_conn_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_limit_conn_module.o \
		src/http/modules/ngx_http_limit_conn_module.c


objs/src/http/modules/ngx_http_limit_req_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_limit_req_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_limit_req_module.o \
		src/http/modules/ngx_http_limit_req_module.c


objs/src/http/modules/ngx_http_realip_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_realip_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_realip_module.o \
		src/http/modules/ngx_http_realip_module.c


objs/src/http/modules/ngx_http_geo_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_geo_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_geo_module.o \
		src/http/modules/ngx_http_geo_module.c


objs/src/http/modules/ngx_http_map_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_map_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_map_module.o \
		src/http/modules/ngx_http_map_module.c


objs/src/http/modules/ngx_http_split_clients_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_split_clients_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_split_clients_module.o \
		src/http/modules/ngx_http_split_clients_module.c


objs/src/http/modules/ngx_http_referer_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_referer_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_referer_module.o \
		src/http/modules/ngx_http_referer_module.c


objs/src/http/modules/ngx_http_rewrite_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_rewrite_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_rewrite_module.o \
		src/http/modules/ngx_http_rewrite_module.c


objs/src/http/modules/ngx_http_ssl_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_ssl_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_ssl_module.o \
		src/http/modules/ngx_http_ssl_module.c


objs/src/http/modules/ngx_http_proxy_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_proxy_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_proxy_module.o \
		src/http/modules/ngx_http_proxy_module.c


objs/src/http/modules/ngx_http_fastcgi_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_fastcgi_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_fastcgi_module.o \
		src/http/modules/ngx_http_fastcgi_module.c


objs/src/http/modules/ngx_http_uwsgi_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_uwsgi_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_uwsgi_module.o \
		src/http/modules/ngx_http_uwsgi_module.c


objs/src/http/modules/ngx_http_scgi_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_scgi_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_scgi_module.o \
		src/http/modules/ngx_http_scgi_module.c


objs/src/http/modules/ngx_http_grpc_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_grpc_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_grpc_module.o \
		src/http/modules/ngx_http_grpc_module.c


objs/src/http/modules/ngx_http_memcached_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_memcached_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_memcached_module.o \
		src/http/modules/ngx_http_memcached_module.c


objs/src/http/modules/ngx_http_empty_gif_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_empty_gif_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_empty_gif_module.o \
		src/http/modules/ngx_http_empty_gif_module.c


objs/src/http/modules/ngx_http_browser_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_browser_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_browser_module.o \
		src/http/modules/ngx_http_browser_module.c


objs/src/http/modules/ngx_http_secure_link_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_secure_link_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_secure_link_module.o \
		src/http/modules/ngx_http_secure_link_module.c


objs/src/http/modules/ngx_http_flv_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_flv_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_flv_module.o \
		src/http/modules/ngx_http_flv_module.c


objs/src/http/modules/ngx_http_mp4_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_mp4_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_mp4_module.o \
		src/http/modules/ngx_http_mp4_module.c


objs/src/http/modules/ngx_http_upstream_hash_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_upstream_hash_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_upstream_hash_module.o \
		src/http/modules/ngx_http_upstream_hash_module.c


objs/src/http/modules/ngx_http_upstream_ip_hash_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_upstream_ip_hash_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_upstream_ip_hash_module.o \
		src/http/modules/ngx_http_upstream_ip_hash_module.c


objs/src/http/modules/ngx_http_upstream_least_conn_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_upstream_least_conn_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_upstream_least_conn_module.o \
		src/http/modules/ngx_http_upstream_least_conn_module.c


objs/src/http/modules/ngx_http_upstream_random_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_upstream_random_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_upstream_random_module.o \
		src/http/modules/ngx_http_upstream_random_module.c


objs/src/http/modules/ngx_http_upstream_keepalive_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_upstream_keepalive_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_upstream_keepalive_module.o \
		src/http/modules/ngx_http_upstream_keepalive_module.c


objs/src/http/modules/ngx_http_upstream_zone_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_upstream_zone_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_upstream_zone_module.o \
		src/http/modules/ngx_http_upstream_zone_module.c


objs/src/http/modules/ngx_http_stub_status_module.o:	$(CORE_DEPS) $(HTTP_DEPS) \
	src/http/modules/ngx_http_stub_status_module.c
	$(CC) -c $(CFLAGS) $(CORE_INCS) $(HTTP_INCS) \
		-o objs/src/http/modules/ngx_http_stub_status_module.o \
		src/http/modules/ngx_http_stub_status_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp.c


objs/addon/nginx-rtmp-module/ngx_rtmp_init.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_init.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_init.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_init.c


objs/addon/nginx-rtmp-module/ngx_rtmp_handshake.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_handshake.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_handshake.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_handshake.c


objs/addon/nginx-rtmp-module/ngx_rtmp_handler.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_handler.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_handler.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_handler.c


objs/addon/nginx-rtmp-module/ngx_rtmp_amf.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_amf.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_amf.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_amf.c


objs/addon/nginx-rtmp-module/ngx_rtmp_send.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_send.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_send.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_send.c


objs/addon/nginx-rtmp-module/ngx_rtmp_shared.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_shared.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_shared.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_shared.c


objs/addon/nginx-rtmp-module/ngx_rtmp_eval.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_eval.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_eval.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_eval.c


objs/addon/nginx-rtmp-module/ngx_rtmp_receive.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_receive.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_receive.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_receive.c


objs/addon/nginx-rtmp-module/ngx_rtmp_core_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_core_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_core_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_core_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_cmd_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_cmd_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_cmd_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_cmd_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_codec_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_codec_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_codec_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_codec_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_access_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_access_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_access_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_access_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_record_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_record_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_record_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_record_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_live_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_live_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_live_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_live_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_play_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_play_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_play_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_play_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_flv_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_flv_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_flv_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_flv_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_mp4_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_mp4_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_mp4_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_mp4_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_netcall_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_netcall_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_netcall_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_netcall_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_relay_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_relay_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_relay_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_relay_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_bandwidth.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_bandwidth.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_bandwidth.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_bandwidth.c


objs/addon/nginx-rtmp-module/ngx_rtmp_exec_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_exec_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_exec_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_exec_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_auto_push_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_auto_push_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_auto_push_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_auto_push_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_notify_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_notify_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_notify_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_notify_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_log_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_log_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_log_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_log_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_limit_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_limit_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_limit_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_limit_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_bitop.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_bitop.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_bitop.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_bitop.c


objs/addon/nginx-rtmp-module/ngx_rtmp_proxy_protocol.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_proxy_protocol.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_proxy_protocol.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_proxy_protocol.c


objs/addon/hls/ngx_rtmp_hls_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/hls/ngx_rtmp_hls_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/hls/ngx_rtmp_hls_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/hls/ngx_rtmp_hls_module.c


objs/addon/dash/ngx_rtmp_dash_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/dash/ngx_rtmp_dash_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/dash/ngx_rtmp_dash_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/dash/ngx_rtmp_dash_module.c


objs/addon/hls/ngx_rtmp_mpegts.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/hls/ngx_rtmp_mpegts.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/hls/ngx_rtmp_mpegts.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/hls/ngx_rtmp_mpegts.c


objs/addon/dash/ngx_rtmp_mp4.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/dash/ngx_rtmp_mp4.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/dash/ngx_rtmp_mp4.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/dash/ngx_rtmp_mp4.c


objs/addon/nginx-rtmp-module/ngx_rtmp_stat_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_stat_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_stat_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_stat_module.c


objs/addon/nginx-rtmp-module/ngx_rtmp_control_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_control_module.c
	$(CC) -c $(CFLAGS)  $(ALL_INCS) \
		-o objs/addon/nginx-rtmp-module/ngx_rtmp_control_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module/ngx_rtmp_control_module.c


modules:	objs/ngx_http_xslt_filter_module.so

objs/ngx_http_xslt_filter_module.so:	objs/src/http/modules/ngx_http_xslt_filter_module.o \
	objs/ngx_http_xslt_filter_module_modules.o

	$(LINK) -o objs/ngx_http_xslt_filter_module.so \
	objs/src/http/modules/ngx_http_xslt_filter_module.o \
	objs/ngx_http_xslt_filter_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC -lxml2 -lxslt -lexslt \
	-shared


objs/ngx_http_xslt_filter_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_http_xslt_filter_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_http_xslt_filter_module_modules.o \
		objs/ngx_http_xslt_filter_module_modules.c


objs/src/http/modules/ngx_http_xslt_filter_module.o:	$(ADDON_DEPS) \
	src/http/modules/ngx_http_xslt_filter_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/http/modules/ngx_http_xslt_filter_module.o \
		src/http/modules/ngx_http_xslt_filter_module.c


modules:	objs/ngx_http_image_filter_module.so

objs/ngx_http_image_filter_module.so:	objs/src/http/modules/ngx_http_image_filter_module.o \
	objs/ngx_http_image_filter_module_modules.o

	$(LINK) -o objs/ngx_http_image_filter_module.so \
	objs/src/http/modules/ngx_http_image_filter_module.o \
	objs/ngx_http_image_filter_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC -lgd \
	-shared


objs/ngx_http_image_filter_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_http_image_filter_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_http_image_filter_module_modules.o \
		objs/ngx_http_image_filter_module_modules.c


objs/src/http/modules/ngx_http_image_filter_module.o:	$(ADDON_DEPS) \
	src/http/modules/ngx_http_image_filter_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/http/modules/ngx_http_image_filter_module.o \
		src/http/modules/ngx_http_image_filter_module.c


modules:	objs/ngx_http_geoip_module.so

objs/ngx_http_geoip_module.so:	objs/src/http/modules/ngx_http_geoip_module.o \
	objs/ngx_http_geoip_module_modules.o

	$(LINK) -o objs/ngx_http_geoip_module.so \
	objs/src/http/modules/ngx_http_geoip_module.o \
	objs/ngx_http_geoip_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC -lGeoIP \
	-shared


objs/ngx_http_geoip_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_http_geoip_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_http_geoip_module_modules.o \
		objs/ngx_http_geoip_module_modules.c


objs/src/http/modules/ngx_http_geoip_module.o:	$(ADDON_DEPS) \
	src/http/modules/ngx_http_geoip_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/http/modules/ngx_http_geoip_module.o \
		src/http/modules/ngx_http_geoip_module.c


modules:	objs/ngx_http_perl_module.so

objs/ngx_http_perl_module.so:	objs/src/http/modules/perl/ngx_http_perl_module.o \
	objs/ngx_http_perl_module_modules.o

	$(LINK) -o objs/ngx_http_perl_module.so \
	objs/src/http/modules/perl/ngx_http_perl_module.o \
	objs/ngx_http_perl_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC -Wl,-E -fstack-protector-strong -L/usr/local/lib -L/usr/lib/x86_64-linux-gnu/perl/5.32/CORE -lperl -ldl -lm -lpthread -lc -lcrypt \
	-shared


objs/ngx_http_perl_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_http_perl_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_http_perl_module_modules.o \
		objs/ngx_http_perl_module_modules.c


objs/src/http/modules/perl/ngx_http_perl_module.o:	$(ADDON_DEPS) \
	src/http/modules/perl/ngx_http_perl_module.c
	$(CC) -c -fPIC $(NGX_PERL_CFLAGS) $(ALL_INCS) \
		-o objs/src/http/modules/perl/ngx_http_perl_module.o \
		src/http/modules/perl/ngx_http_perl_module.c


modules:	objs/ngx_stream_geoip_module.so

objs/ngx_stream_geoip_module.so:	objs/src/stream/ngx_stream_geoip_module.o \
	objs/ngx_stream_geoip_module_modules.o

	$(LINK) -o objs/ngx_stream_geoip_module.so \
	objs/src/stream/ngx_stream_geoip_module.o \
	objs/ngx_stream_geoip_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC -lGeoIP \
	-shared


objs/ngx_stream_geoip_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_stream_geoip_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_stream_geoip_module_modules.o \
		objs/ngx_stream_geoip_module_modules.c


objs/src/stream/ngx_stream_geoip_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_geoip_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_geoip_module.o \
		src/stream/ngx_stream_geoip_module.c


modules:	objs/ngx_http_headers_more_filter_module.so

objs/ngx_http_headers_more_filter_module.so:	objs/addon/src/ngx_http_headers_more_filter_module.o \
	objs/addon/src/ngx_http_headers_more_headers_out.o \
	objs/addon/src/ngx_http_headers_more_headers_in.o \
	objs/addon/src/ngx_http_headers_more_util.o \
	objs/ngx_http_headers_more_filter_module_modules.o

	$(LINK) -o objs/ngx_http_headers_more_filter_module.so \
	objs/addon/src/ngx_http_headers_more_filter_module.o \
	objs/addon/src/ngx_http_headers_more_headers_out.o \
	objs/addon/src/ngx_http_headers_more_headers_in.o \
	objs/addon/src/ngx_http_headers_more_util.o \
	objs/ngx_http_headers_more_filter_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC \
	-shared


objs/ngx_http_headers_more_filter_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_http_headers_more_filter_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_http_headers_more_filter_module_modules.o \
		objs/ngx_http_headers_more_filter_module_modules.c


objs/addon/src/ngx_http_headers_more_filter_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-headers-more-filter/src/ngx_http_headers_more_filter_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_headers_more_filter_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-headers-more-filter/src/ngx_http_headers_more_filter_module.c


objs/addon/src/ngx_http_headers_more_headers_out.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-headers-more-filter/src/ngx_http_headers_more_headers_out.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_headers_more_headers_out.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-headers-more-filter/src/ngx_http_headers_more_headers_out.c


objs/addon/src/ngx_http_headers_more_headers_in.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-headers-more-filter/src/ngx_http_headers_more_headers_in.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_headers_more_headers_in.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-headers-more-filter/src/ngx_http_headers_more_headers_in.c


objs/addon/src/ngx_http_headers_more_util.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-headers-more-filter/src/ngx_http_headers_more_util.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_headers_more_util.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-headers-more-filter/src/ngx_http_headers_more_util.c


modules:	objs/ngx_http_auth_pam_module.so

objs/ngx_http_auth_pam_module.so:	objs/addon/http-auth-pam/ngx_http_auth_pam_module.o \
	objs/ngx_http_auth_pam_module_modules.o

	$(LINK) -o objs/ngx_http_auth_pam_module.so \
	objs/addon/http-auth-pam/ngx_http_auth_pam_module.o \
	objs/ngx_http_auth_pam_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC -lpam \
	-shared


objs/ngx_http_auth_pam_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_http_auth_pam_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_http_auth_pam_module_modules.o \
		objs/ngx_http_auth_pam_module_modules.c


objs/addon/http-auth-pam/ngx_http_auth_pam_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-auth-pam/ngx_http_auth_pam_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/http-auth-pam/ngx_http_auth_pam_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-auth-pam/ngx_http_auth_pam_module.c


modules:	objs/ngx_http_cache_purge_module.so

objs/ngx_http_cache_purge_module.so:	objs/addon/http-cache-purge/ngx_cache_purge_module.o \
	objs/ngx_http_cache_purge_module_modules.o

	$(LINK) -o objs/ngx_http_cache_purge_module.so \
	objs/addon/http-cache-purge/ngx_cache_purge_module.o \
	objs/ngx_http_cache_purge_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC \
	-shared


objs/ngx_http_cache_purge_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_http_cache_purge_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_http_cache_purge_module_modules.o \
		objs/ngx_http_cache_purge_module_modules.c


objs/addon/http-cache-purge/ngx_cache_purge_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-cache-purge/ngx_cache_purge_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/http-cache-purge/ngx_cache_purge_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-cache-purge/ngx_cache_purge_module.c


modules:	objs/ngx_http_dav_ext_module.so

objs/ngx_http_dav_ext_module.so:	objs/addon/http-dav-ext/ngx_http_dav_ext_module.o \
	objs/ngx_http_dav_ext_module_modules.o

	$(LINK) -o objs/ngx_http_dav_ext_module.so \
	objs/addon/http-dav-ext/ngx_http_dav_ext_module.o \
	objs/ngx_http_dav_ext_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC -lxml2 -lxslt -lexslt \
	-shared


objs/ngx_http_dav_ext_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_http_dav_ext_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_http_dav_ext_module_modules.o \
		objs/ngx_http_dav_ext_module_modules.c


objs/addon/http-dav-ext/ngx_http_dav_ext_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-dav-ext/ngx_http_dav_ext_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/http-dav-ext/ngx_http_dav_ext_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-dav-ext/ngx_http_dav_ext_module.c


modules:	objs/ndk_http_module.so

objs/ndk_http_module.so:	objs/addon/src/ndk.o \
	objs/ndk_http_module_modules.o

	$(LINK) -o objs/ndk_http_module.so \
	objs/addon/src/ndk.o \
	objs/ndk_http_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC \
	-shared


objs/ndk_http_module_modules.o:	$(CORE_DEPS) \
	objs/ndk_http_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ndk_http_module_modules.o \
		objs/ndk_http_module_modules.c


objs/addon/src/ndk.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-ndk/src/ndk.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ndk.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-ndk/src/ndk.c


modules:	objs/ngx_http_echo_module.so

objs/ngx_http_echo_module.so:	objs/addon/src/ngx_http_echo_module.o \
	objs/addon/src/ngx_http_echo_util.o \
	objs/addon/src/ngx_http_echo_timer.o \
	objs/addon/src/ngx_http_echo_var.o \
	objs/addon/src/ngx_http_echo_handler.o \
	objs/addon/src/ngx_http_echo_filter.o \
	objs/addon/src/ngx_http_echo_sleep.o \
	objs/addon/src/ngx_http_echo_location.o \
	objs/addon/src/ngx_http_echo_echo.o \
	objs/addon/src/ngx_http_echo_request_info.o \
	objs/addon/src/ngx_http_echo_subrequest.o \
	objs/addon/src/ngx_http_echo_foreach.o \
	objs/ngx_http_echo_module_modules.o

	$(LINK) -o objs/ngx_http_echo_module.so \
	objs/addon/src/ngx_http_echo_module.o \
	objs/addon/src/ngx_http_echo_util.o \
	objs/addon/src/ngx_http_echo_timer.o \
	objs/addon/src/ngx_http_echo_var.o \
	objs/addon/src/ngx_http_echo_handler.o \
	objs/addon/src/ngx_http_echo_filter.o \
	objs/addon/src/ngx_http_echo_sleep.o \
	objs/addon/src/ngx_http_echo_location.o \
	objs/addon/src/ngx_http_echo_echo.o \
	objs/addon/src/ngx_http_echo_request_info.o \
	objs/addon/src/ngx_http_echo_subrequest.o \
	objs/addon/src/ngx_http_echo_foreach.o \
	objs/ngx_http_echo_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC \
	-shared


objs/ngx_http_echo_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_http_echo_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_http_echo_module_modules.o \
		objs/ngx_http_echo_module_modules.c


objs/addon/src/ngx_http_echo_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_echo_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_module.c


objs/addon/src/ngx_http_echo_util.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_util.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_echo_util.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_util.c


objs/addon/src/ngx_http_echo_timer.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_timer.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_echo_timer.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_timer.c


objs/addon/src/ngx_http_echo_var.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_var.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_echo_var.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_var.c


objs/addon/src/ngx_http_echo_handler.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_handler.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_echo_handler.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_handler.c


objs/addon/src/ngx_http_echo_filter.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_filter.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_echo_filter.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_filter.c


objs/addon/src/ngx_http_echo_sleep.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_sleep.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_echo_sleep.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_sleep.c


objs/addon/src/ngx_http_echo_location.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_location.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_echo_location.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_location.c


objs/addon/src/ngx_http_echo_echo.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_echo.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_echo_echo.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_echo.c


objs/addon/src/ngx_http_echo_request_info.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_request_info.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_echo_request_info.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_request_info.c


objs/addon/src/ngx_http_echo_subrequest.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_subrequest.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_echo_subrequest.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_subrequest.c


objs/addon/src/ngx_http_echo_foreach.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_foreach.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_echo_foreach.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-echo/src/ngx_http_echo_foreach.c


modules:	objs/ngx_http_fancyindex_module.so

objs/ngx_http_fancyindex_module.so:	objs/addon/http-fancyindex/ngx_http_fancyindex_module.o \
	objs/ngx_http_fancyindex_module_modules.o

	$(LINK) -o objs/ngx_http_fancyindex_module.so \
	objs/addon/http-fancyindex/ngx_http_fancyindex_module.o \
	objs/ngx_http_fancyindex_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC \
	-shared


objs/ngx_http_fancyindex_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_http_fancyindex_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_http_fancyindex_module_modules.o \
		objs/ngx_http_fancyindex_module_modules.c


objs/addon/http-fancyindex/ngx_http_fancyindex_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-fancyindex/ngx_http_fancyindex_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/http-fancyindex/ngx_http_fancyindex_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-fancyindex/ngx_http_fancyindex_module.c


modules:	objs/ngx_http_geoip2_module.so

objs/ngx_http_geoip2_module.so:	objs/addon/http-geoip2/ngx_http_geoip2_module.o \
	objs/ngx_http_geoip2_module_modules.o

	$(LINK) -o objs/ngx_http_geoip2_module.so \
	objs/addon/http-geoip2/ngx_http_geoip2_module.o \
	objs/ngx_http_geoip2_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC -lmaxminddb \
	-shared


objs/ngx_http_geoip2_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_http_geoip2_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_http_geoip2_module_modules.o \
		objs/ngx_http_geoip2_module_modules.c


objs/addon/http-geoip2/ngx_http_geoip2_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-geoip2/ngx_http_geoip2_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/http-geoip2/ngx_http_geoip2_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-geoip2/ngx_http_geoip2_module.c


modules:	objs/ngx_stream_geoip2_module.so

objs/ngx_stream_geoip2_module.so:	objs/addon/http-geoip2/ngx_stream_geoip2_module.o \
	objs/ngx_stream_geoip2_module_modules.o

	$(LINK) -o objs/ngx_stream_geoip2_module.so \
	objs/addon/http-geoip2/ngx_stream_geoip2_module.o \
	objs/ngx_stream_geoip2_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC -lmaxminddb \
	-shared


objs/ngx_stream_geoip2_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_stream_geoip2_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_stream_geoip2_module_modules.o \
		objs/ngx_stream_geoip2_module_modules.c


objs/addon/http-geoip2/ngx_stream_geoip2_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-geoip2/ngx_stream_geoip2_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/http-geoip2/ngx_stream_geoip2_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-geoip2/ngx_stream_geoip2_module.c


modules:	objs/ngx_nchan_module.so

objs/ngx_nchan_module.so:	objs/addon/src/nchan_defs.o \
	objs/addon/src/nchan_variables.o \
	objs/addon/src/nchan_module.o \
	objs/addon/util/nchan_debug.o \
	objs/addon/util/nchan_list.o \
	objs/addon/util/nchan_slist.o \
	objs/addon/util/ngx_nchan_hacked_slab.o \
	objs/addon/util/shmem.o \
	objs/addon/util/nchan_rbtree.o \
	objs/addon/util/nchan_reuse_queue.o \
	objs/addon/util/nchan_output.o \
	objs/addon/util/nchan_util.o \
	objs/addon/util/nchan_fake_request.o \
	objs/addon/util/nchan_bufchainpool.o \
	objs/addon/util/nchan_channel_id.o \
	objs/addon/util/nchan_output_info.o \
	objs/addon/util/nchan_msg.o \
	objs/addon/util/nchan_thingcache.o \
	objs/addon/util/nchan_reaper.o \
	objs/addon/util/nchan_subrequest.o \
	objs/addon/util/nchan_benchmark.o \
	objs/addon/util/hdr_histogram.o \
	objs/addon/subscribers/common.o \
	objs/addon/subscribers/longpoll.o \
	objs/addon/subscribers/intervalpoll.o \
	objs/addon/subscribers/eventsource.o \
	objs/addon/subscribers/http-chunked.o \
	objs/addon/subscribers/http-multipart-mixed.o \
	objs/addon/subscribers/http-raw-stream.o \
	objs/addon/subscribers/websocket.o \
	objs/addon/src/nchan_websocket_publisher.o \
	objs/addon/subscribers/internal.o \
	objs/addon/subscribers/memstore_ipc.o \
	objs/addon/subscribers/memstore_multi.o \
	objs/addon/subscribers/memstore_redis.o \
	objs/addon/subscribers/getmsg_proxy.o \
	objs/addon/subscribers/benchmark.o \
	objs/addon/store/spool.o \
	objs/addon/store/ngx_rwlock.o \
	objs/addon/store/store_common.o \
	objs/addon/memory/ipc.o \
	objs/addon/memory/ipc-handlers.o \
	objs/addon/memory/groups.o \
	objs/addon/memory/memstore.o \
	objs/addon/hiredis/hiredis.o \
	objs/addon/hiredis/read.o \
	objs/addon/hiredis/async.o \
	objs/addon/hiredis/sds.o \
	objs/addon/hiredis/net.o \
	objs/addon/redis/cmp.o \
	objs/addon/redis/redis_lua_commands.o \
	objs/addon/redis/redis_nodeset_parser.o \
	objs/addon/redis/redis_nodeset.o \
	objs/addon/redis/rdsstore.o \
	objs/addon/redis/redis_nginx_adapter.o \
	objs/ngx_nchan_module_modules.o

	$(LINK) -o objs/ngx_nchan_module.so \
	objs/addon/src/nchan_defs.o \
	objs/addon/src/nchan_variables.o \
	objs/addon/src/nchan_module.o \
	objs/addon/util/nchan_debug.o \
	objs/addon/util/nchan_list.o \
	objs/addon/util/nchan_slist.o \
	objs/addon/util/ngx_nchan_hacked_slab.o \
	objs/addon/util/shmem.o \
	objs/addon/util/nchan_rbtree.o \
	objs/addon/util/nchan_reuse_queue.o \
	objs/addon/util/nchan_output.o \
	objs/addon/util/nchan_util.o \
	objs/addon/util/nchan_fake_request.o \
	objs/addon/util/nchan_bufchainpool.o \
	objs/addon/util/nchan_channel_id.o \
	objs/addon/util/nchan_output_info.o \
	objs/addon/util/nchan_msg.o \
	objs/addon/util/nchan_thingcache.o \
	objs/addon/util/nchan_reaper.o \
	objs/addon/util/nchan_subrequest.o \
	objs/addon/util/nchan_benchmark.o \
	objs/addon/util/hdr_histogram.o \
	objs/addon/subscribers/common.o \
	objs/addon/subscribers/longpoll.o \
	objs/addon/subscribers/intervalpoll.o \
	objs/addon/subscribers/eventsource.o \
	objs/addon/subscribers/http-chunked.o \
	objs/addon/subscribers/http-multipart-mixed.o \
	objs/addon/subscribers/http-raw-stream.o \
	objs/addon/subscribers/websocket.o \
	objs/addon/src/nchan_websocket_publisher.o \
	objs/addon/subscribers/internal.o \
	objs/addon/subscribers/memstore_ipc.o \
	objs/addon/subscribers/memstore_multi.o \
	objs/addon/subscribers/memstore_redis.o \
	objs/addon/subscribers/getmsg_proxy.o \
	objs/addon/subscribers/benchmark.o \
	objs/addon/store/spool.o \
	objs/addon/store/ngx_rwlock.o \
	objs/addon/store/store_common.o \
	objs/addon/memory/ipc.o \
	objs/addon/memory/ipc-handlers.o \
	objs/addon/memory/groups.o \
	objs/addon/memory/memstore.o \
	objs/addon/hiredis/hiredis.o \
	objs/addon/hiredis/read.o \
	objs/addon/hiredis/async.o \
	objs/addon/hiredis/sds.o \
	objs/addon/hiredis/net.o \
	objs/addon/redis/cmp.o \
	objs/addon/redis/redis_lua_commands.o \
	objs/addon/redis/redis_nodeset_parser.o \
	objs/addon/redis/redis_nodeset.o \
	objs/addon/redis/rdsstore.o \
	objs/addon/redis/redis_nginx_adapter.o \
	objs/ngx_nchan_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC -lm \
	-shared


objs/ngx_nchan_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_nchan_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_nchan_module_modules.o \
		objs/ngx_nchan_module_modules.c


objs/addon/src/nchan_defs.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/nchan_defs.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/nchan_defs.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/nchan_defs.c


objs/addon/src/nchan_variables.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/nchan_variables.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/nchan_variables.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/nchan_variables.c


objs/addon/src/nchan_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/nchan_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/nchan_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/nchan_module.c


objs/addon/util/nchan_debug.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_debug.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/nchan_debug.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_debug.c


objs/addon/util/nchan_list.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_list.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/nchan_list.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_list.c


objs/addon/util/nchan_slist.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_slist.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/nchan_slist.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_slist.c


objs/addon/util/ngx_nchan_hacked_slab.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/ngx_nchan_hacked_slab.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/ngx_nchan_hacked_slab.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/ngx_nchan_hacked_slab.c


objs/addon/util/shmem.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/shmem.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/shmem.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/shmem.c


objs/addon/util/nchan_rbtree.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_rbtree.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/nchan_rbtree.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_rbtree.c


objs/addon/util/nchan_reuse_queue.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_reuse_queue.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/nchan_reuse_queue.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_reuse_queue.c


objs/addon/util/nchan_output.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_output.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/nchan_output.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_output.c


objs/addon/util/nchan_util.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_util.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/nchan_util.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_util.c


objs/addon/util/nchan_fake_request.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_fake_request.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/nchan_fake_request.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_fake_request.c


objs/addon/util/nchan_bufchainpool.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_bufchainpool.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/nchan_bufchainpool.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_bufchainpool.c


objs/addon/util/nchan_channel_id.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_channel_id.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/nchan_channel_id.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_channel_id.c


objs/addon/util/nchan_output_info.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_output_info.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/nchan_output_info.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_output_info.c


objs/addon/util/nchan_msg.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_msg.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/nchan_msg.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_msg.c


objs/addon/util/nchan_thingcache.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_thingcache.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/nchan_thingcache.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_thingcache.c


objs/addon/util/nchan_reaper.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_reaper.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/nchan_reaper.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_reaper.c


objs/addon/util/nchan_subrequest.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_subrequest.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/nchan_subrequest.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_subrequest.c


objs/addon/util/nchan_benchmark.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_benchmark.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/nchan_benchmark.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/nchan_benchmark.c


objs/addon/util/hdr_histogram.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/hdr_histogram.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/util/hdr_histogram.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/util/hdr_histogram.c


objs/addon/subscribers/common.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/common.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/subscribers/common.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/common.c


objs/addon/subscribers/longpoll.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/longpoll.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/subscribers/longpoll.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/longpoll.c


objs/addon/subscribers/intervalpoll.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/intervalpoll.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/subscribers/intervalpoll.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/intervalpoll.c


objs/addon/subscribers/eventsource.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/eventsource.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/subscribers/eventsource.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/eventsource.c


objs/addon/subscribers/http-chunked.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/http-chunked.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/subscribers/http-chunked.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/http-chunked.c


objs/addon/subscribers/http-multipart-mixed.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/http-multipart-mixed.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/subscribers/http-multipart-mixed.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/http-multipart-mixed.c


objs/addon/subscribers/http-raw-stream.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/http-raw-stream.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/subscribers/http-raw-stream.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/http-raw-stream.c


objs/addon/subscribers/websocket.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/websocket.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/subscribers/websocket.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/websocket.c


objs/addon/src/nchan_websocket_publisher.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/nchan_websocket_publisher.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/nchan_websocket_publisher.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/nchan_websocket_publisher.c


objs/addon/subscribers/internal.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/internal.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/subscribers/internal.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/internal.c


objs/addon/subscribers/memstore_ipc.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/memstore_ipc.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/subscribers/memstore_ipc.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/memstore_ipc.c


objs/addon/subscribers/memstore_multi.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/memstore_multi.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/subscribers/memstore_multi.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/memstore_multi.c


objs/addon/subscribers/memstore_redis.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/memstore_redis.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/subscribers/memstore_redis.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/memstore_redis.c


objs/addon/subscribers/getmsg_proxy.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/getmsg_proxy.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/subscribers/getmsg_proxy.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/getmsg_proxy.c


objs/addon/subscribers/benchmark.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/benchmark.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/subscribers/benchmark.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/subscribers/benchmark.c


objs/addon/store/spool.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/spool.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/store/spool.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/spool.c


objs/addon/store/ngx_rwlock.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/ngx_rwlock.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/store/ngx_rwlock.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/ngx_rwlock.c


objs/addon/store/store_common.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/store_common.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/store/store_common.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/store_common.c


objs/addon/memory/ipc.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/memory/ipc.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/memory/ipc.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/memory/ipc.c


objs/addon/memory/ipc-handlers.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/memory/ipc-handlers.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/memory/ipc-handlers.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/memory/ipc-handlers.c


objs/addon/memory/groups.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/memory/groups.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/memory/groups.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/memory/groups.c


objs/addon/memory/memstore.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/memory/memstore.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/memory/memstore.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/memory/memstore.c


objs/addon/hiredis/hiredis.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/hiredis/hiredis.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/hiredis/hiredis.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/hiredis/hiredis.c


objs/addon/hiredis/read.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/hiredis/read.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/hiredis/read.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/hiredis/read.c


objs/addon/hiredis/async.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/hiredis/async.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/hiredis/async.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/hiredis/async.c


objs/addon/hiredis/sds.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/hiredis/sds.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/hiredis/sds.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/hiredis/sds.c


objs/addon/hiredis/net.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/hiredis/net.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/hiredis/net.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/hiredis/net.c


objs/addon/redis/cmp.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/cmp.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/redis/cmp.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/cmp.c


objs/addon/redis/redis_lua_commands.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/redis_lua_commands.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/redis/redis_lua_commands.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/redis_lua_commands.c


objs/addon/redis/redis_nodeset_parser.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/redis_nodeset_parser.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/redis/redis_nodeset_parser.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/redis_nodeset_parser.c


objs/addon/redis/redis_nodeset.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/redis_nodeset.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/redis/redis_nodeset.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/redis_nodeset.c


objs/addon/redis/rdsstore.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/rdsstore.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/redis/rdsstore.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/rdsstore.c


objs/addon/redis/redis_nginx_adapter.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/redis_nginx_adapter.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/redis/redis_nginx_adapter.o \
		/root/ngx/nginx-1.18.0/debian/modules/nchan/src/store/redis/redis_nginx_adapter.c


modules:	objs/ngx_http_lua_module.so

objs/ngx_http_lua_module.so:	objs/addon/src/ngx_http_lua_script.o \
	objs/addon/src/ngx_http_lua_log.o \
	objs/addon/src/ngx_http_lua_subrequest.o \
	objs/addon/src/ngx_http_lua_ndk.o \
	objs/addon/src/ngx_http_lua_control.o \
	objs/addon/src/ngx_http_lua_time.o \
	objs/addon/src/ngx_http_lua_misc.o \
	objs/addon/src/ngx_http_lua_variable.o \
	objs/addon/src/ngx_http_lua_string.o \
	objs/addon/src/ngx_http_lua_output.o \
	objs/addon/src/ngx_http_lua_headers.o \
	objs/addon/src/ngx_http_lua_req_body.o \
	objs/addon/src/ngx_http_lua_uri.o \
	objs/addon/src/ngx_http_lua_args.o \
	objs/addon/src/ngx_http_lua_ctx.o \
	objs/addon/src/ngx_http_lua_regex.o \
	objs/addon/src/ngx_http_lua_module.o \
	objs/addon/src/ngx_http_lua_headers_out.o \
	objs/addon/src/ngx_http_lua_headers_in.o \
	objs/addon/src/ngx_http_lua_directive.o \
	objs/addon/src/ngx_http_lua_consts.o \
	objs/addon/src/ngx_http_lua_exception.o \
	objs/addon/src/ngx_http_lua_util.o \
	objs/addon/src/ngx_http_lua_cache.o \
	objs/addon/src/ngx_http_lua_contentby.o \
	objs/addon/src/ngx_http_lua_rewriteby.o \
	objs/addon/src/ngx_http_lua_accessby.o \
	objs/addon/src/ngx_http_lua_setby.o \
	objs/addon/src/ngx_http_lua_capturefilter.o \
	objs/addon/src/ngx_http_lua_clfactory.o \
	objs/addon/src/ngx_http_lua_pcrefix.o \
	objs/addon/src/ngx_http_lua_headerfilterby.o \
	objs/addon/src/ngx_http_lua_shdict.o \
	objs/addon/src/ngx_http_lua_socket_tcp.o \
	objs/addon/src/ngx_http_lua_api.o \
	objs/addon/src/ngx_http_lua_logby.o \
	objs/addon/src/ngx_http_lua_sleep.o \
	objs/addon/src/ngx_http_lua_semaphore.o \
	objs/addon/src/ngx_http_lua_coroutine.o \
	objs/addon/src/ngx_http_lua_bodyfilterby.o \
	objs/addon/src/ngx_http_lua_initby.o \
	objs/addon/src/ngx_http_lua_initworkerby.o \
	objs/addon/src/ngx_http_lua_socket_udp.o \
	objs/addon/src/ngx_http_lua_req_method.o \
	objs/addon/src/ngx_http_lua_phase.o \
	objs/addon/src/ngx_http_lua_uthread.o \
	objs/addon/src/ngx_http_lua_timer.o \
	objs/addon/src/ngx_http_lua_config.o \
	objs/addon/src/ngx_http_lua_worker.o \
	objs/addon/src/ngx_http_lua_ssl_certby.o \
	objs/addon/src/ngx_http_lua_ssl_ocsp.o \
	objs/addon/src/ngx_http_lua_lex.o \
	objs/addon/src/ngx_http_lua_balancer.o \
	objs/addon/src/ngx_http_lua_ssl_session_storeby.o \
	objs/addon/src/ngx_http_lua_ssl_session_fetchby.o \
	objs/addon/src/ngx_http_lua_ssl.o \
	objs/addon/src/ngx_http_lua_log_ringbuf.o \
	objs/ngx_http_lua_module_modules.o

	$(LINK) -o objs/ngx_http_lua_module.so \
	objs/addon/src/ngx_http_lua_script.o \
	objs/addon/src/ngx_http_lua_log.o \
	objs/addon/src/ngx_http_lua_subrequest.o \
	objs/addon/src/ngx_http_lua_ndk.o \
	objs/addon/src/ngx_http_lua_control.o \
	objs/addon/src/ngx_http_lua_time.o \
	objs/addon/src/ngx_http_lua_misc.o \
	objs/addon/src/ngx_http_lua_variable.o \
	objs/addon/src/ngx_http_lua_string.o \
	objs/addon/src/ngx_http_lua_output.o \
	objs/addon/src/ngx_http_lua_headers.o \
	objs/addon/src/ngx_http_lua_req_body.o \
	objs/addon/src/ngx_http_lua_uri.o \
	objs/addon/src/ngx_http_lua_args.o \
	objs/addon/src/ngx_http_lua_ctx.o \
	objs/addon/src/ngx_http_lua_regex.o \
	objs/addon/src/ngx_http_lua_module.o \
	objs/addon/src/ngx_http_lua_headers_out.o \
	objs/addon/src/ngx_http_lua_headers_in.o \
	objs/addon/src/ngx_http_lua_directive.o \
	objs/addon/src/ngx_http_lua_consts.o \
	objs/addon/src/ngx_http_lua_exception.o \
	objs/addon/src/ngx_http_lua_util.o \
	objs/addon/src/ngx_http_lua_cache.o \
	objs/addon/src/ngx_http_lua_contentby.o \
	objs/addon/src/ngx_http_lua_rewriteby.o \
	objs/addon/src/ngx_http_lua_accessby.o \
	objs/addon/src/ngx_http_lua_setby.o \
	objs/addon/src/ngx_http_lua_capturefilter.o \
	objs/addon/src/ngx_http_lua_clfactory.o \
	objs/addon/src/ngx_http_lua_pcrefix.o \
	objs/addon/src/ngx_http_lua_headerfilterby.o \
	objs/addon/src/ngx_http_lua_shdict.o \
	objs/addon/src/ngx_http_lua_socket_tcp.o \
	objs/addon/src/ngx_http_lua_api.o \
	objs/addon/src/ngx_http_lua_logby.o \
	objs/addon/src/ngx_http_lua_sleep.o \
	objs/addon/src/ngx_http_lua_semaphore.o \
	objs/addon/src/ngx_http_lua_coroutine.o \
	objs/addon/src/ngx_http_lua_bodyfilterby.o \
	objs/addon/src/ngx_http_lua_initby.o \
	objs/addon/src/ngx_http_lua_initworkerby.o \
	objs/addon/src/ngx_http_lua_socket_udp.o \
	objs/addon/src/ngx_http_lua_req_method.o \
	objs/addon/src/ngx_http_lua_phase.o \
	objs/addon/src/ngx_http_lua_uthread.o \
	objs/addon/src/ngx_http_lua_timer.o \
	objs/addon/src/ngx_http_lua_config.o \
	objs/addon/src/ngx_http_lua_worker.o \
	objs/addon/src/ngx_http_lua_ssl_certby.o \
	objs/addon/src/ngx_http_lua_ssl_ocsp.o \
	objs/addon/src/ngx_http_lua_lex.o \
	objs/addon/src/ngx_http_lua_balancer.o \
	objs/addon/src/ngx_http_lua_ssl_session_storeby.o \
	objs/addon/src/ngx_http_lua_ssl_session_fetchby.o \
	objs/addon/src/ngx_http_lua_ssl.o \
	objs/addon/src/ngx_http_lua_log_ringbuf.o \
	objs/ngx_http_lua_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC -L/usr/lib -lm -lluajit-5.1 -ldl \
	-shared


objs/ngx_http_lua_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_http_lua_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_http_lua_module_modules.o \
		objs/ngx_http_lua_module_modules.c


objs/addon/src/ngx_http_lua_script.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_script.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_script.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_script.c


objs/addon/src/ngx_http_lua_log.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_log.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_log.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_log.c


objs/addon/src/ngx_http_lua_subrequest.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_subrequest.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_subrequest.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_subrequest.c


objs/addon/src/ngx_http_lua_ndk.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ndk.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_ndk.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ndk.c


objs/addon/src/ngx_http_lua_control.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_control.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_control.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_control.c


objs/addon/src/ngx_http_lua_time.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_time.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_time.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_time.c


objs/addon/src/ngx_http_lua_misc.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_misc.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_misc.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_misc.c


objs/addon/src/ngx_http_lua_variable.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_variable.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_variable.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_variable.c


objs/addon/src/ngx_http_lua_string.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_string.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_string.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_string.c


objs/addon/src/ngx_http_lua_output.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_output.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_output.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_output.c


objs/addon/src/ngx_http_lua_headers.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_headers.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_headers.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_headers.c


objs/addon/src/ngx_http_lua_req_body.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_req_body.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_req_body.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_req_body.c


objs/addon/src/ngx_http_lua_uri.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_uri.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_uri.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_uri.c


objs/addon/src/ngx_http_lua_args.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_args.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_args.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_args.c


objs/addon/src/ngx_http_lua_ctx.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ctx.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_ctx.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ctx.c


objs/addon/src/ngx_http_lua_regex.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_regex.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_regex.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_regex.c


objs/addon/src/ngx_http_lua_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_module.c


objs/addon/src/ngx_http_lua_headers_out.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_headers_out.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_headers_out.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_headers_out.c


objs/addon/src/ngx_http_lua_headers_in.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_headers_in.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_headers_in.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_headers_in.c


objs/addon/src/ngx_http_lua_directive.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_directive.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_directive.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_directive.c


objs/addon/src/ngx_http_lua_consts.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_consts.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_consts.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_consts.c


objs/addon/src/ngx_http_lua_exception.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_exception.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_exception.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_exception.c


objs/addon/src/ngx_http_lua_util.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_util.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_util.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_util.c


objs/addon/src/ngx_http_lua_cache.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_cache.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_cache.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_cache.c


objs/addon/src/ngx_http_lua_contentby.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_contentby.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_contentby.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_contentby.c


objs/addon/src/ngx_http_lua_rewriteby.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_rewriteby.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_rewriteby.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_rewriteby.c


objs/addon/src/ngx_http_lua_accessby.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_accessby.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_accessby.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_accessby.c


objs/addon/src/ngx_http_lua_setby.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_setby.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_setby.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_setby.c


objs/addon/src/ngx_http_lua_capturefilter.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_capturefilter.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_capturefilter.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_capturefilter.c


objs/addon/src/ngx_http_lua_clfactory.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_clfactory.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_clfactory.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_clfactory.c


objs/addon/src/ngx_http_lua_pcrefix.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_pcrefix.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_pcrefix.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_pcrefix.c


objs/addon/src/ngx_http_lua_headerfilterby.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_headerfilterby.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_headerfilterby.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_headerfilterby.c


objs/addon/src/ngx_http_lua_shdict.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_shdict.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_shdict.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_shdict.c


objs/addon/src/ngx_http_lua_socket_tcp.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_socket_tcp.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_socket_tcp.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_socket_tcp.c


objs/addon/src/ngx_http_lua_api.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_api.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_api.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_api.c


objs/addon/src/ngx_http_lua_logby.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_logby.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_logby.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_logby.c


objs/addon/src/ngx_http_lua_sleep.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_sleep.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_sleep.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_sleep.c


objs/addon/src/ngx_http_lua_semaphore.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_semaphore.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_semaphore.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_semaphore.c


objs/addon/src/ngx_http_lua_coroutine.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_coroutine.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_coroutine.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_coroutine.c


objs/addon/src/ngx_http_lua_bodyfilterby.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_bodyfilterby.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_bodyfilterby.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_bodyfilterby.c


objs/addon/src/ngx_http_lua_initby.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_initby.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_initby.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_initby.c


objs/addon/src/ngx_http_lua_initworkerby.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_initworkerby.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_initworkerby.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_initworkerby.c


objs/addon/src/ngx_http_lua_socket_udp.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_socket_udp.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_socket_udp.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_socket_udp.c


objs/addon/src/ngx_http_lua_req_method.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_req_method.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_req_method.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_req_method.c


objs/addon/src/ngx_http_lua_phase.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_phase.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_phase.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_phase.c


objs/addon/src/ngx_http_lua_uthread.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_uthread.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_uthread.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_uthread.c


objs/addon/src/ngx_http_lua_timer.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_timer.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_timer.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_timer.c


objs/addon/src/ngx_http_lua_config.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_config.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_config.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_config.c


objs/addon/src/ngx_http_lua_worker.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_worker.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_worker.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_worker.c


objs/addon/src/ngx_http_lua_ssl_certby.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ssl_certby.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_ssl_certby.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ssl_certby.c


objs/addon/src/ngx_http_lua_ssl_ocsp.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ssl_ocsp.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_ssl_ocsp.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ssl_ocsp.c


objs/addon/src/ngx_http_lua_lex.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_lex.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_lex.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_lex.c


objs/addon/src/ngx_http_lua_balancer.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_balancer.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_balancer.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_balancer.c


objs/addon/src/ngx_http_lua_ssl_session_storeby.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ssl_session_storeby.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_ssl_session_storeby.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ssl_session_storeby.c


objs/addon/src/ngx_http_lua_ssl_session_fetchby.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ssl_session_fetchby.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_ssl_session_fetchby.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ssl_session_fetchby.c


objs/addon/src/ngx_http_lua_ssl.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ssl.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_ssl.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_ssl.c


objs/addon/src/ngx_http_lua_log_ringbuf.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_log_ringbuf.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/src/ngx_http_lua_log_ringbuf.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-lua/src/ngx_http_lua_log_ringbuf.c


modules:	objs/ngx_rtmp_module.so

objs/ngx_rtmp_module.so:	objs/addon/rtmp/ngx_rtmp.o \
	objs/addon/rtmp/ngx_rtmp_init.o \
	objs/addon/rtmp/ngx_rtmp_handshake.o \
	objs/addon/rtmp/ngx_rtmp_handler.o \
	objs/addon/rtmp/ngx_rtmp_amf.o \
	objs/addon/rtmp/ngx_rtmp_send.o \
	objs/addon/rtmp/ngx_rtmp_shared.o \
	objs/addon/rtmp/ngx_rtmp_eval.o \
	objs/addon/rtmp/ngx_rtmp_receive.o \
	objs/addon/rtmp/ngx_rtmp_core_module.o \
	objs/addon/rtmp/ngx_rtmp_cmd_module.o \
	objs/addon/rtmp/ngx_rtmp_codec_module.o \
	objs/addon/rtmp/ngx_rtmp_access_module.o \
	objs/addon/rtmp/ngx_rtmp_record_module.o \
	objs/addon/rtmp/ngx_rtmp_live_module.o \
	objs/addon/rtmp/ngx_rtmp_play_module.o \
	objs/addon/rtmp/ngx_rtmp_flv_module.o \
	objs/addon/rtmp/ngx_rtmp_mp4_module.o \
	objs/addon/rtmp/ngx_rtmp_netcall_module.o \
	objs/addon/rtmp/ngx_rtmp_relay_module.o \
	objs/addon/rtmp/ngx_rtmp_bandwidth.o \
	objs/addon/rtmp/ngx_rtmp_exec_module.o \
	objs/addon/rtmp/ngx_rtmp_auto_push_module.o \
	objs/addon/rtmp/ngx_rtmp_notify_module.o \
	objs/addon/rtmp/ngx_rtmp_log_module.o \
	objs/addon/rtmp/ngx_rtmp_limit_module.o \
	objs/addon/rtmp/ngx_rtmp_bitop.o \
	objs/addon/rtmp/ngx_rtmp_proxy_protocol.o \
	objs/addon/hls/ngx_rtmp_hls_module.o \
	objs/addon/dash/ngx_rtmp_dash_module.o \
	objs/addon/hls/ngx_rtmp_mpegts.o \
	objs/addon/dash/ngx_rtmp_mp4.o \
	objs/addon/rtmp/ngx_rtmp_stat_module.o \
	objs/addon/rtmp/ngx_rtmp_control_module.o \
	objs/ngx_rtmp_module_modules.o

	$(LINK) -o objs/ngx_rtmp_module.so \
	objs/addon/rtmp/ngx_rtmp.o \
	objs/addon/rtmp/ngx_rtmp_init.o \
	objs/addon/rtmp/ngx_rtmp_handshake.o \
	objs/addon/rtmp/ngx_rtmp_handler.o \
	objs/addon/rtmp/ngx_rtmp_amf.o \
	objs/addon/rtmp/ngx_rtmp_send.o \
	objs/addon/rtmp/ngx_rtmp_shared.o \
	objs/addon/rtmp/ngx_rtmp_eval.o \
	objs/addon/rtmp/ngx_rtmp_receive.o \
	objs/addon/rtmp/ngx_rtmp_core_module.o \
	objs/addon/rtmp/ngx_rtmp_cmd_module.o \
	objs/addon/rtmp/ngx_rtmp_codec_module.o \
	objs/addon/rtmp/ngx_rtmp_access_module.o \
	objs/addon/rtmp/ngx_rtmp_record_module.o \
	objs/addon/rtmp/ngx_rtmp_live_module.o \
	objs/addon/rtmp/ngx_rtmp_play_module.o \
	objs/addon/rtmp/ngx_rtmp_flv_module.o \
	objs/addon/rtmp/ngx_rtmp_mp4_module.o \
	objs/addon/rtmp/ngx_rtmp_netcall_module.o \
	objs/addon/rtmp/ngx_rtmp_relay_module.o \
	objs/addon/rtmp/ngx_rtmp_bandwidth.o \
	objs/addon/rtmp/ngx_rtmp_exec_module.o \
	objs/addon/rtmp/ngx_rtmp_auto_push_module.o \
	objs/addon/rtmp/ngx_rtmp_notify_module.o \
	objs/addon/rtmp/ngx_rtmp_log_module.o \
	objs/addon/rtmp/ngx_rtmp_limit_module.o \
	objs/addon/rtmp/ngx_rtmp_bitop.o \
	objs/addon/rtmp/ngx_rtmp_proxy_protocol.o \
	objs/addon/hls/ngx_rtmp_hls_module.o \
	objs/addon/dash/ngx_rtmp_dash_module.o \
	objs/addon/hls/ngx_rtmp_mpegts.o \
	objs/addon/dash/ngx_rtmp_mp4.o \
	objs/addon/rtmp/ngx_rtmp_stat_module.o \
	objs/addon/rtmp/ngx_rtmp_control_module.o \
	objs/ngx_rtmp_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC \
	-shared


objs/ngx_rtmp_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_rtmp_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_rtmp_module_modules.o \
		objs/ngx_rtmp_module_modules.c


objs/addon/rtmp/ngx_rtmp.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp.c


objs/addon/rtmp/ngx_rtmp_init.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_init.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_init.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_init.c


objs/addon/rtmp/ngx_rtmp_handshake.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_handshake.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_handshake.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_handshake.c


objs/addon/rtmp/ngx_rtmp_handler.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_handler.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_handler.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_handler.c


objs/addon/rtmp/ngx_rtmp_amf.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_amf.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_amf.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_amf.c


objs/addon/rtmp/ngx_rtmp_send.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_send.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_send.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_send.c


objs/addon/rtmp/ngx_rtmp_shared.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_shared.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_shared.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_shared.c


objs/addon/rtmp/ngx_rtmp_eval.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_eval.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_eval.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_eval.c


objs/addon/rtmp/ngx_rtmp_receive.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_receive.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_receive.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_receive.c


objs/addon/rtmp/ngx_rtmp_core_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_core_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_core_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_core_module.c


objs/addon/rtmp/ngx_rtmp_cmd_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_cmd_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_cmd_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_cmd_module.c


objs/addon/rtmp/ngx_rtmp_codec_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_codec_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_codec_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_codec_module.c


objs/addon/rtmp/ngx_rtmp_access_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_access_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_access_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_access_module.c


objs/addon/rtmp/ngx_rtmp_record_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_record_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_record_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_record_module.c


objs/addon/rtmp/ngx_rtmp_live_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_live_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_live_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_live_module.c


objs/addon/rtmp/ngx_rtmp_play_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_play_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_play_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_play_module.c


objs/addon/rtmp/ngx_rtmp_flv_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_flv_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_flv_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_flv_module.c


objs/addon/rtmp/ngx_rtmp_mp4_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_mp4_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_mp4_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_mp4_module.c


objs/addon/rtmp/ngx_rtmp_netcall_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_netcall_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_netcall_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_netcall_module.c


objs/addon/rtmp/ngx_rtmp_relay_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_relay_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_relay_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_relay_module.c


objs/addon/rtmp/ngx_rtmp_bandwidth.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_bandwidth.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_bandwidth.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_bandwidth.c


objs/addon/rtmp/ngx_rtmp_exec_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_exec_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_exec_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_exec_module.c


objs/addon/rtmp/ngx_rtmp_auto_push_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_auto_push_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_auto_push_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_auto_push_module.c


objs/addon/rtmp/ngx_rtmp_notify_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_notify_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_notify_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_notify_module.c


objs/addon/rtmp/ngx_rtmp_log_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_log_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_log_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_log_module.c


objs/addon/rtmp/ngx_rtmp_limit_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_limit_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_limit_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_limit_module.c


objs/addon/rtmp/ngx_rtmp_bitop.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_bitop.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_bitop.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_bitop.c


objs/addon/rtmp/ngx_rtmp_proxy_protocol.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_proxy_protocol.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_proxy_protocol.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_proxy_protocol.c


objs/addon/hls/ngx_rtmp_hls_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/hls/ngx_rtmp_hls_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/hls/ngx_rtmp_hls_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/hls/ngx_rtmp_hls_module.c


objs/addon/dash/ngx_rtmp_dash_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/dash/ngx_rtmp_dash_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/dash/ngx_rtmp_dash_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/dash/ngx_rtmp_dash_module.c


objs/addon/hls/ngx_rtmp_mpegts.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/hls/ngx_rtmp_mpegts.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/hls/ngx_rtmp_mpegts.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/hls/ngx_rtmp_mpegts.c


objs/addon/dash/ngx_rtmp_mp4.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/dash/ngx_rtmp_mp4.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/dash/ngx_rtmp_mp4.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/dash/ngx_rtmp_mp4.c


objs/addon/rtmp/ngx_rtmp_stat_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_stat_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_stat_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_stat_module.c


objs/addon/rtmp/ngx_rtmp_control_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_control_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/rtmp/ngx_rtmp_control_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/rtmp/ngx_rtmp_control_module.c


modules:	objs/ngx_http_uploadprogress_module.so

objs/ngx_http_uploadprogress_module.so:	objs/addon/http-uploadprogress/ngx_http_uploadprogress_module.o \
	objs/ngx_http_uploadprogress_module_modules.o

	$(LINK) -o objs/ngx_http_uploadprogress_module.so \
	objs/addon/http-uploadprogress/ngx_http_uploadprogress_module.o \
	objs/ngx_http_uploadprogress_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC \
	-shared


objs/ngx_http_uploadprogress_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_http_uploadprogress_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_http_uploadprogress_module_modules.o \
		objs/ngx_http_uploadprogress_module_modules.c


objs/addon/http-uploadprogress/ngx_http_uploadprogress_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-uploadprogress/ngx_http_uploadprogress_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/http-uploadprogress/ngx_http_uploadprogress_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-uploadprogress/ngx_http_uploadprogress_module.c


modules:	objs/ngx_http_upstream_fair_module.so

objs/ngx_http_upstream_fair_module.so:	objs/addon/http-upstream-fair/ngx_http_upstream_fair_module.o \
	objs/ngx_http_upstream_fair_module_modules.o

	$(LINK) -o objs/ngx_http_upstream_fair_module.so \
	objs/addon/http-upstream-fair/ngx_http_upstream_fair_module.o \
	objs/ngx_http_upstream_fair_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC \
	-shared


objs/ngx_http_upstream_fair_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_http_upstream_fair_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_http_upstream_fair_module_modules.o \
		objs/ngx_http_upstream_fair_module_modules.c


objs/addon/http-upstream-fair/ngx_http_upstream_fair_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-upstream-fair/ngx_http_upstream_fair_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/http-upstream-fair/ngx_http_upstream_fair_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-upstream-fair/ngx_http_upstream_fair_module.c


modules:	objs/ngx_http_subs_filter_module.so

objs/ngx_http_subs_filter_module.so:	objs/addon/http-subs-filter/ngx_http_subs_filter_module.o \
	objs/ngx_http_subs_filter_module_modules.o

	$(LINK) -o objs/ngx_http_subs_filter_module.so \
	objs/addon/http-subs-filter/ngx_http_subs_filter_module.o \
	objs/ngx_http_subs_filter_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC \
	-shared


objs/ngx_http_subs_filter_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_http_subs_filter_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_http_subs_filter_module_modules.o \
		objs/ngx_http_subs_filter_module_modules.c


objs/addon/http-subs-filter/ngx_http_subs_filter_module.o:	$(ADDON_DEPS) \
	/root/ngx/nginx-1.18.0/debian/modules/http-subs-filter/ngx_http_subs_filter_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/addon/http-subs-filter/ngx_http_subs_filter_module.o \
		/root/ngx/nginx-1.18.0/debian/modules/http-subs-filter/ngx_http_subs_filter_module.c


modules:	objs/ngx_mail_module.so

objs/ngx_mail_module.so:	objs/src/mail/ngx_mail.o \
	objs/src/mail/ngx_mail_core_module.o \
	objs/src/mail/ngx_mail_handler.o \
	objs/src/mail/ngx_mail_parse.o \
	objs/src/mail/ngx_mail_ssl_module.o \
	objs/src/mail/ngx_mail_pop3_module.o \
	objs/src/mail/ngx_mail_pop3_handler.o \
	objs/src/mail/ngx_mail_imap_module.o \
	objs/src/mail/ngx_mail_imap_handler.o \
	objs/src/mail/ngx_mail_smtp_module.o \
	objs/src/mail/ngx_mail_smtp_handler.o \
	objs/src/mail/ngx_mail_auth_http_module.o \
	objs/src/mail/ngx_mail_proxy_module.o \
	objs/ngx_mail_module_modules.o

	$(LINK) -o objs/ngx_mail_module.so \
	objs/src/mail/ngx_mail.o \
	objs/src/mail/ngx_mail_core_module.o \
	objs/src/mail/ngx_mail_handler.o \
	objs/src/mail/ngx_mail_parse.o \
	objs/src/mail/ngx_mail_ssl_module.o \
	objs/src/mail/ngx_mail_pop3_module.o \
	objs/src/mail/ngx_mail_pop3_handler.o \
	objs/src/mail/ngx_mail_imap_module.o \
	objs/src/mail/ngx_mail_imap_handler.o \
	objs/src/mail/ngx_mail_smtp_module.o \
	objs/src/mail/ngx_mail_smtp_handler.o \
	objs/src/mail/ngx_mail_auth_http_module.o \
	objs/src/mail/ngx_mail_proxy_module.o \
	objs/ngx_mail_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC \
	-shared


objs/ngx_mail_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_mail_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_mail_module_modules.o \
		objs/ngx_mail_module_modules.c


objs/src/mail/ngx_mail.o:	$(ADDON_DEPS) \
	src/mail/ngx_mail.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/mail/ngx_mail.o \
		src/mail/ngx_mail.c


objs/src/mail/ngx_mail_core_module.o:	$(ADDON_DEPS) \
	src/mail/ngx_mail_core_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/mail/ngx_mail_core_module.o \
		src/mail/ngx_mail_core_module.c


objs/src/mail/ngx_mail_handler.o:	$(ADDON_DEPS) \
	src/mail/ngx_mail_handler.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/mail/ngx_mail_handler.o \
		src/mail/ngx_mail_handler.c


objs/src/mail/ngx_mail_parse.o:	$(ADDON_DEPS) \
	src/mail/ngx_mail_parse.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/mail/ngx_mail_parse.o \
		src/mail/ngx_mail_parse.c


objs/src/mail/ngx_mail_ssl_module.o:	$(ADDON_DEPS) \
	src/mail/ngx_mail_ssl_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/mail/ngx_mail_ssl_module.o \
		src/mail/ngx_mail_ssl_module.c


objs/src/mail/ngx_mail_pop3_module.o:	$(ADDON_DEPS) \
	src/mail/ngx_mail_pop3_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/mail/ngx_mail_pop3_module.o \
		src/mail/ngx_mail_pop3_module.c


objs/src/mail/ngx_mail_pop3_handler.o:	$(ADDON_DEPS) \
	src/mail/ngx_mail_pop3_handler.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/mail/ngx_mail_pop3_handler.o \
		src/mail/ngx_mail_pop3_handler.c


objs/src/mail/ngx_mail_imap_module.o:	$(ADDON_DEPS) \
	src/mail/ngx_mail_imap_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/mail/ngx_mail_imap_module.o \
		src/mail/ngx_mail_imap_module.c


objs/src/mail/ngx_mail_imap_handler.o:	$(ADDON_DEPS) \
	src/mail/ngx_mail_imap_handler.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/mail/ngx_mail_imap_handler.o \
		src/mail/ngx_mail_imap_handler.c


objs/src/mail/ngx_mail_smtp_module.o:	$(ADDON_DEPS) \
	src/mail/ngx_mail_smtp_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/mail/ngx_mail_smtp_module.o \
		src/mail/ngx_mail_smtp_module.c


objs/src/mail/ngx_mail_smtp_handler.o:	$(ADDON_DEPS) \
	src/mail/ngx_mail_smtp_handler.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/mail/ngx_mail_smtp_handler.o \
		src/mail/ngx_mail_smtp_handler.c


objs/src/mail/ngx_mail_auth_http_module.o:	$(ADDON_DEPS) \
	src/mail/ngx_mail_auth_http_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/mail/ngx_mail_auth_http_module.o \
		src/mail/ngx_mail_auth_http_module.c


objs/src/mail/ngx_mail_proxy_module.o:	$(ADDON_DEPS) \
	src/mail/ngx_mail_proxy_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/mail/ngx_mail_proxy_module.o \
		src/mail/ngx_mail_proxy_module.c


modules:	objs/ngx_stream_module.so

objs/ngx_stream_module.so:	objs/src/stream/ngx_stream.o \
	objs/src/stream/ngx_stream_variables.o \
	objs/src/stream/ngx_stream_script.o \
	objs/src/stream/ngx_stream_handler.o \
	objs/src/stream/ngx_stream_core_module.o \
	objs/src/stream/ngx_stream_log_module.o \
	objs/src/stream/ngx_stream_proxy_module.o \
	objs/src/stream/ngx_stream_upstream.o \
	objs/src/stream/ngx_stream_upstream_round_robin.o \
	objs/src/stream/ngx_stream_write_filter_module.o \
	objs/src/stream/ngx_stream_ssl_module.o \
	objs/src/stream/ngx_stream_limit_conn_module.o \
	objs/src/stream/ngx_stream_access_module.o \
	objs/src/stream/ngx_stream_geo_module.o \
	objs/src/stream/ngx_stream_map_module.o \
	objs/src/stream/ngx_stream_split_clients_module.o \
	objs/src/stream/ngx_stream_return_module.o \
	objs/src/stream/ngx_stream_upstream_hash_module.o \
	objs/src/stream/ngx_stream_upstream_least_conn_module.o \
	objs/src/stream/ngx_stream_upstream_random_module.o \
	objs/src/stream/ngx_stream_upstream_zone_module.o \
	objs/src/stream/ngx_stream_ssl_preread_module.o \
	objs/ngx_stream_module_modules.o

	$(LINK) -o objs/ngx_stream_module.so \
	objs/src/stream/ngx_stream.o \
	objs/src/stream/ngx_stream_variables.o \
	objs/src/stream/ngx_stream_script.o \
	objs/src/stream/ngx_stream_handler.o \
	objs/src/stream/ngx_stream_core_module.o \
	objs/src/stream/ngx_stream_log_module.o \
	objs/src/stream/ngx_stream_proxy_module.o \
	objs/src/stream/ngx_stream_upstream.o \
	objs/src/stream/ngx_stream_upstream_round_robin.o \
	objs/src/stream/ngx_stream_write_filter_module.o \
	objs/src/stream/ngx_stream_ssl_module.o \
	objs/src/stream/ngx_stream_limit_conn_module.o \
	objs/src/stream/ngx_stream_access_module.o \
	objs/src/stream/ngx_stream_geo_module.o \
	objs/src/stream/ngx_stream_map_module.o \
	objs/src/stream/ngx_stream_split_clients_module.o \
	objs/src/stream/ngx_stream_return_module.o \
	objs/src/stream/ngx_stream_upstream_hash_module.o \
	objs/src/stream/ngx_stream_upstream_least_conn_module.o \
	objs/src/stream/ngx_stream_upstream_random_module.o \
	objs/src/stream/ngx_stream_upstream_zone_module.o \
	objs/src/stream/ngx_stream_ssl_preread_module.o \
	objs/ngx_stream_module_modules.o \
	-Wl,-z,relro -Wl,-z,now -fPIC \
	-shared


objs/ngx_stream_module_modules.o:	$(CORE_DEPS) \
	objs/ngx_stream_module_modules.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/ngx_stream_module_modules.o \
		objs/ngx_stream_module_modules.c


objs/src/stream/ngx_stream.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream.o \
		src/stream/ngx_stream.c


objs/src/stream/ngx_stream_variables.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_variables.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_variables.o \
		src/stream/ngx_stream_variables.c


objs/src/stream/ngx_stream_script.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_script.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_script.o \
		src/stream/ngx_stream_script.c


objs/src/stream/ngx_stream_handler.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_handler.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_handler.o \
		src/stream/ngx_stream_handler.c


objs/src/stream/ngx_stream_core_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_core_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_core_module.o \
		src/stream/ngx_stream_core_module.c


objs/src/stream/ngx_stream_log_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_log_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_log_module.o \
		src/stream/ngx_stream_log_module.c


objs/src/stream/ngx_stream_proxy_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_proxy_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_proxy_module.o \
		src/stream/ngx_stream_proxy_module.c


objs/src/stream/ngx_stream_upstream.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_upstream.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_upstream.o \
		src/stream/ngx_stream_upstream.c


objs/src/stream/ngx_stream_upstream_round_robin.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_upstream_round_robin.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_upstream_round_robin.o \
		src/stream/ngx_stream_upstream_round_robin.c


objs/src/stream/ngx_stream_write_filter_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_write_filter_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_write_filter_module.o \
		src/stream/ngx_stream_write_filter_module.c


objs/src/stream/ngx_stream_ssl_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_ssl_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_ssl_module.o \
		src/stream/ngx_stream_ssl_module.c


objs/src/stream/ngx_stream_limit_conn_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_limit_conn_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_limit_conn_module.o \
		src/stream/ngx_stream_limit_conn_module.c


objs/src/stream/ngx_stream_access_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_access_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_access_module.o \
		src/stream/ngx_stream_access_module.c


objs/src/stream/ngx_stream_geo_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_geo_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_geo_module.o \
		src/stream/ngx_stream_geo_module.c


objs/src/stream/ngx_stream_map_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_map_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_map_module.o \
		src/stream/ngx_stream_map_module.c


objs/src/stream/ngx_stream_split_clients_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_split_clients_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_split_clients_module.o \
		src/stream/ngx_stream_split_clients_module.c


objs/src/stream/ngx_stream_return_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_return_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_return_module.o \
		src/stream/ngx_stream_return_module.c


objs/src/stream/ngx_stream_upstream_hash_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_upstream_hash_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_upstream_hash_module.o \
		src/stream/ngx_stream_upstream_hash_module.c


objs/src/stream/ngx_stream_upstream_least_conn_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_upstream_least_conn_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_upstream_least_conn_module.o \
		src/stream/ngx_stream_upstream_least_conn_module.c


objs/src/stream/ngx_stream_upstream_random_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_upstream_random_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_upstream_random_module.o \
		src/stream/ngx_stream_upstream_random_module.c


objs/src/stream/ngx_stream_upstream_zone_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_upstream_zone_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_upstream_zone_module.o \
		src/stream/ngx_stream_upstream_zone_module.c


objs/src/stream/ngx_stream_ssl_preread_module.o:	$(ADDON_DEPS) \
	src/stream/ngx_stream_ssl_preread_module.c
	$(CC) -c -fPIC $(CFLAGS) $(ALL_INCS) \
		-o objs/src/stream/ngx_stream_ssl_preread_module.o \
		src/stream/ngx_stream_ssl_preread_module.c


objs/src/http/modules/perl/ngx_http_perl_module.o: \
		objs/src/http/modules/perl/blib/arch/auto/nginx/nginx.so

objs/src/http/modules/perl/blib/arch/auto/nginx/nginx.so: \
		$(CORE_DEPS) $(HTTP_DEPS) \
		src/http/modules/perl/ngx_http_perl_module.h \
		objs/src/http/modules/perl/Makefile
	cd objs/src/http/modules/perl && $(MAKE)

	rm -rf objs/install_perl


objs/src/http/modules/perl/Makefile: \
		objs/ngx_auto_config.h \
		src/core/nginx.h \
		src/http/modules/perl/Makefile.PL \
		src/http/modules/perl/nginx.pm \
		src/http/modules/perl/nginx.xs \
		src/http/modules/perl/typemap
	grep 'define NGINX_VERSION' src/core/nginx.h \
		| sed -e 's/^.*"\(.*\)".*/\1/' > \
		objs/src/http/modules/perl/version
	sed "s/%%VERSION%%/`cat objs/src/http/modules/perl/version`/" \
		src/http/modules/perl/nginx.pm > \
		objs/src/http/modules/perl/nginx.pm
	cp -p src/http/modules/perl/nginx.xs objs/src/http/modules/perl/
	cp -p src/http/modules/perl/typemap objs/src/http/modules/perl/
	cp -p src/http/modules/perl/Makefile.PL objs/src/http/modules/perl/

	cd objs/src/http/modules/perl \
		&& NGX_PM_CFLAGS="$(NGX_PM_CFLAGS) -g -g -O2 -ffile-prefix-map=/root/ngx/nginx-1.18.0=. -fstack-protector-strong -Wformat -Werror=format-security -fPIC -Wdate-time -D_FORTIFY_SOURCE=2" \
			NGX_PM_LDFLAGS=" -Wl,-z,relro -Wl,-z,now -fPIC $(NGX_PM_LDFLAGS)" \
			NGX_INCS="src/core src/event src/event/modules src/os/unix src/http/modules/perl /root/ngx/nginx-1.18.0/debian/modules/nginx-rtmp-module /root/ngx/nginx-1.18.0/debian/modules/http-ndk/objs objs/addon/ndk /root/ngx/nginx-1.18.0/debian/modules/http-ndk/src /root/ngx/nginx-1.18.0/debian/modules/http-ndk/objs objs/addon/ndk /root/ngx/nginx-1.18.0/debian/modules/nchan/src /root/ngx/nginx-1.18.0/debian/modules/http-lua/src/api  /usr/include/luajit-2.1 /root/ngx/nginx-1.18.0/debian/modules/rtmp   /usr/include/libxml2   objs  src/http src/http/modules src/http/v2 /root/ngx/nginx-1.18.0/debian/modules/http-ndk/src " \
			NGX_DEPS="$(CORE_DEPS) $(HTTP_DEPS)" \
		perl Makefile.PL \
			LIB= \
			INSTALLSITEMAN3DIR=


install_perl_modules:
	cd objs/src/http/modules/perl && $(MAKE) install

manpage:	objs/nginx.8

objs/nginx.8:	man/nginx.8 objs/ngx_auto_config.h
	sed -e "s|%%PREFIX%%|/usr/share/nginx|" \
		-e "s|%%PID_PATH%%|/run/nginx.pid|" \
		-e "s|%%CONF_PATH%%|/etc/nginx/nginx.conf|" \
		-e "s|%%ERROR_LOG_PATH%%|/var/log/nginx/error.log|" \
		< man/nginx.8 > $@

install:	build install_perl_modules
	test -d '$(DESTDIR)/usr/share/nginx' || mkdir -p '$(DESTDIR)/usr/share/nginx'

	test -d '$(DESTDIR)/usr/share/nginx/sbin' \
		|| mkdir -p '$(DESTDIR)/usr/share/nginx/sbin'
	test ! -f '$(DESTDIR)/usr/share/nginx/sbin/nginx' \
		|| mv '$(DESTDIR)/usr/share/nginx/sbin/nginx' \
			'$(DESTDIR)/usr/share/nginx/sbin/nginx.old'
	cp objs/nginx '$(DESTDIR)/usr/share/nginx/sbin/nginx'

	test -d '$(DESTDIR)/etc/nginx' \
		|| mkdir -p '$(DESTDIR)/etc/nginx'

	cp conf/koi-win '$(DESTDIR)/etc/nginx'
	cp conf/koi-utf '$(DESTDIR)/etc/nginx'
	cp conf/win-utf '$(DESTDIR)/etc/nginx'

	test -f '$(DESTDIR)/etc/nginx/mime.types' \
		|| cp conf/mime.types '$(DESTDIR)/etc/nginx'
	cp conf/mime.types '$(DESTDIR)/etc/nginx/mime.types.default'

	test -f '$(DESTDIR)/etc/nginx/fastcgi_params' \
		|| cp conf/fastcgi_params '$(DESTDIR)/etc/nginx'
	cp conf/fastcgi_params \
		'$(DESTDIR)/etc/nginx/fastcgi_params.default'

	test -f '$(DESTDIR)/etc/nginx/fastcgi.conf' \
		|| cp conf/fastcgi.conf '$(DESTDIR)/etc/nginx'
	cp conf/fastcgi.conf '$(DESTDIR)/etc/nginx/fastcgi.conf.default'

	test -f '$(DESTDIR)/etc/nginx/uwsgi_params' \
		|| cp conf/uwsgi_params '$(DESTDIR)/etc/nginx'
	cp conf/uwsgi_params \
		'$(DESTDIR)/etc/nginx/uwsgi_params.default'

	test -f '$(DESTDIR)/etc/nginx/scgi_params' \
		|| cp conf/scgi_params '$(DESTDIR)/etc/nginx'
	cp conf/scgi_params \
		'$(DESTDIR)/etc/nginx/scgi_params.default'

	test -f '$(DESTDIR)/etc/nginx/nginx.conf' \
		|| cp conf/nginx.conf '$(DESTDIR)/etc/nginx/nginx.conf'
	cp conf/nginx.conf '$(DESTDIR)/etc/nginx/nginx.conf.default'

	test -d '$(DESTDIR)/run' \
		|| mkdir -p '$(DESTDIR)/run'

	test -d '$(DESTDIR)/var/log/nginx' \
		|| mkdir -p '$(DESTDIR)/var/log/nginx'

	test -d '$(DESTDIR)/usr/share/nginx/html' \
		|| cp -R docs/html '$(DESTDIR)/usr/share/nginx'

	test -d '$(DESTDIR)/var/log/nginx' \
		|| mkdir -p '$(DESTDIR)/var/log/nginx'

	test -d '$(DESTDIR)/usr/lib/nginx/modules' \
		|| mkdir -p '$(DESTDIR)/usr/lib/nginx/modules'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_xslt_filter_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_xslt_filter_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_http_xslt_filter_module.so.old'
	cp objs/ngx_http_xslt_filter_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_xslt_filter_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_image_filter_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_image_filter_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_http_image_filter_module.so.old'
	cp objs/ngx_http_image_filter_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_image_filter_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_geoip_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_geoip_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_http_geoip_module.so.old'
	cp objs/ngx_http_geoip_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_geoip_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_perl_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_perl_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_http_perl_module.so.old'
	cp objs/ngx_http_perl_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_perl_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_stream_geoip_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_stream_geoip_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_stream_geoip_module.so.old'
	cp objs/ngx_stream_geoip_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_stream_geoip_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_headers_more_filter_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_headers_more_filter_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_http_headers_more_filter_module.so.old'
	cp objs/ngx_http_headers_more_filter_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_headers_more_filter_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_auth_pam_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_auth_pam_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_http_auth_pam_module.so.old'
	cp objs/ngx_http_auth_pam_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_auth_pam_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_cache_purge_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_cache_purge_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_http_cache_purge_module.so.old'
	cp objs/ngx_http_cache_purge_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_cache_purge_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_dav_ext_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_dav_ext_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_http_dav_ext_module.so.old'
	cp objs/ngx_http_dav_ext_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_dav_ext_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ndk_http_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ndk_http_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ndk_http_module.so.old'
	cp objs/ndk_http_module.so '$(DESTDIR)/usr/lib/nginx/modules/ndk_http_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_echo_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_echo_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_http_echo_module.so.old'
	cp objs/ngx_http_echo_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_echo_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_fancyindex_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_fancyindex_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_http_fancyindex_module.so.old'
	cp objs/ngx_http_fancyindex_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_fancyindex_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_geoip2_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_geoip2_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_http_geoip2_module.so.old'
	cp objs/ngx_http_geoip2_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_geoip2_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_stream_geoip2_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_stream_geoip2_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_stream_geoip2_module.so.old'
	cp objs/ngx_stream_geoip2_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_stream_geoip2_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_nchan_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_nchan_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_nchan_module.so.old'
	cp objs/ngx_nchan_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_nchan_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_lua_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_lua_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_http_lua_module.so.old'
	cp objs/ngx_http_lua_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_lua_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_rtmp_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_rtmp_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_rtmp_module.so.old'
	cp objs/ngx_rtmp_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_rtmp_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_uploadprogress_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_uploadprogress_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_http_uploadprogress_module.so.old'
	cp objs/ngx_http_uploadprogress_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_uploadprogress_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_upstream_fair_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_upstream_fair_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_http_upstream_fair_module.so.old'
	cp objs/ngx_http_upstream_fair_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_upstream_fair_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_subs_filter_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_subs_filter_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_http_subs_filter_module.so.old'
	cp objs/ngx_http_subs_filter_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_http_subs_filter_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_mail_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_mail_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_mail_module.so.old'
	cp objs/ngx_mail_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_mail_module.so'

	test ! -f '$(DESTDIR)/usr/lib/nginx/modules/ngx_stream_module.so' \
		|| mv '$(DESTDIR)/usr/lib/nginx/modules/ngx_stream_module.so' \
			'$(DESTDIR)/usr/lib/nginx/modules/ngx_stream_module.so.old'
	cp objs/ngx_stream_module.so '$(DESTDIR)/usr/lib/nginx/modules/ngx_stream_module.so'
