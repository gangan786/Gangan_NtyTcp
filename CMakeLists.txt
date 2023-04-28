cmake_minimum_required(VERSION 3.17)
project(Gangan_NtyTcp C)

set(CMAKE_C_STANDARD 11)

include_directories(include)

add_executable(Gangan_NtyTcp
        app/nty_example_epoll_rb_server.c
        app/nty_example_epoll_server.c
        app/nty_example_posix_block_server.c
        app/nty_example_tcp_server.c
        include/nty_addr.h
        include/nty_api.h
        include/nty_arp.h
        include/nty_buffer.h
        include/nty_config.h
        include/nty_epoll.h
        include/nty_epoll_inner.h
        include/nty_hash.h
        include/nty_header.h
        include/nty_mempool.h
        include/nty_nic.h
        include/nty_queue.h
        include/nty_socket.h
        include/nty_tcp.h
        include/nty_timer.h
        include/nty_tree.h
        src/nty_addr.c
        src/nty_api.c
        src/nty_arp.c
        src/nty_buffer.c
        src/nty_epoll.c
        src/nty_epoll_rb.c
        src/nty_eth.c
        src/nty_hash.c
        src/nty_icmp.c
        src/nty_ip.c
        src/nty_mempool.c
        src/nty_nic.c
        src/nty_socket.c
        src/nty_stream.c
        src/nty_tcp.c
        src/nty_timer.c
        src/nty_udp.c)
