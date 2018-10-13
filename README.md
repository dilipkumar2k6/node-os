# os module

## os.cpus()
It gives cup details.
```
os.cpus()
```
```
[ { model: 'Intel(R) Core(TM) i7-3540M CPU @ 3.00GHz',
    speed: 3000,
    times: { user: 6787340, nice: 0, sys: 4475380, idle: 25182620, irq: 0 } },
  { model: 'Intel(R) Core(TM) i7-3540M CPU @ 3.00GHz',
    speed: 3000,
    times: { user: 4069990, nice: 0, sys: 1994730, idle: 30379610, irq: 0 } },
  { model: 'Intel(R) Core(TM) i7-3540M CPU @ 3.00GHz',
    speed: 3000,
    times: { user: 6417070, nice: 0, sys: 3819800, idle: 26207470, irq: 0 } },
  { model: 'Intel(R) Core(TM) i7-3540M CPU @ 3.00GHz',
    speed: 3000,
    times: { user: 4086740, nice: 0, sys: 1931110, idle: 30426480, irq: 0 } } ]

```

## os.networkInterfaces
It gives network details.

```
os.networkInterfaces()
```
```
{ lo0:
   [ { address: '127.0.0.1',
       netmask: '255.0.0.0',
       family: 'IPv4',
       mac: '00:00:00:00:00:00',
       internal: true,
       cidr: '127.0.0.1/8' },
     { address: '::1',
       netmask: 'ffff:ffff:ffff:ffff:ffff:ffff:ffff:ffff',
       family: 'IPv6',
       mac: '00:00:00:00:00:00',
       scopeid: 0,
       internal: true,
       cidr: '::1/128' },
     { address: 'fe80::1',
       netmask: 'ffff:ffff:ffff:ffff::',
       family: 'IPv6',
       mac: '00:00:00:00:00:00',
       scopeid: 1,
       internal: true,
       cidr: 'fe80::1/64' } ],
  en0:
   [ { address: 'fe80::1087:f3af:d371:62ca',
       netmask: 'ffff:ffff:ffff:ffff::',
       family: 'IPv6',
       mac: '54:26:96:d0:d4:f7',
       scopeid: 7,
       internal: false,
       cidr: 'fe80::1087:f3af:d371:62ca/64' },
     { address: '192.168.0.12',
       netmask: '255.255.255.0',
       family: 'IPv4',
       mac: '54:26:96:d0:d4:f7',
       internal: false,
       cidr: '192.168.0.12/24' },
     { address: '2600:8800:b04:4c00:14f6:ed75:ee23:eff',
       netmask: 'ffff:ffff:ffff:ffff::',
       family: 'IPv6',
       mac: '54:26:96:d0:d4:f7',
       scopeid: 0,
       internal: false,
       cidr: '2600:8800:b04:4c00:14f6:ed75:ee23:eff/64' },
     { address: '2600:8800:b04:4c00:70c1:5adc:b995:95ae',
       netmask: 'ffff:ffff:ffff:ffff::',
       family: 'IPv6',
       mac: '54:26:96:d0:d4:f7',
       scopeid: 0,
       internal: false,
       cidr: '2600:8800:b04:4c00:70c1:5adc:b995:95ae/64' } ],
  awdl0:
   [ { address: 'fe80::9055:bff:fe3e:e5e1',
       netmask: 'ffff:ffff:ffff:ffff::',
       family: 'IPv6',
       mac: '92:55:0b:3e:e5:e1',
       scopeid: 9,
       internal: false,
       cidr: 'fe80::9055:bff:fe3e:e5e1/64' } ],
  utun0:
   [ { address: 'fe80::48c3:dd94:fd55:c9e5',
       netmask: 'ffff:ffff:ffff:ffff::',
       family: 'IPv6',
       mac: '00:00:00:00:00:00',
       scopeid: 13,
       internal: false,
       cidr: 'fe80::48c3:dd94:fd55:c9e5/64' } ] }

```

## os.freemem
It gives available free memory.
```
> os.freemem()
132296704
```

## os.type
It gives what Operation system was node compiled for.
```
> os.type()
'Darwin'
```
## os.release
It returns the release version of operating system.
```
> os.release()
'17.7.0'
```
## os.userInfo
It returns details about logged in user.
```
> os.userInfo()
{ uid: 501,
  gid: 20,
  username: 'dilipkumar',
  homedir: '/Users/dilipkumar',
  shell: '/bin/zsh' }
```
## os.constants
It returns all the predefined constants
```
> os.constants
{ UV_UDP_REUSEADDR: 4,
  dlopen: { RTLD_LAZY: 1, RTLD_NOW: 2, RTLD_GLOBAL: 8, RTLD_LOCAL: 4 },
  errno:
   { E2BIG: 7,
     EACCES: 13,
     EADDRINUSE: 48,
     EADDRNOTAVAIL: 49,
     EAFNOSUPPORT: 47,
     EAGAIN: 35,
     EALREADY: 37,
     EBADF: 9,
     EBADMSG: 94,
     EBUSY: 16,
     ECANCELED: 89,
     ECHILD: 10,
     ECONNABORTED: 53,
     ECONNREFUSED: 61,
     ECONNRESET: 54,
     EDEADLK: 11,
     EDESTADDRREQ: 39,
     EDOM: 33,
     EDQUOT: 69,
     EEXIST: 17,
     EFAULT: 14,
     EFBIG: 27,
     EHOSTUNREACH: 65,
     EIDRM: 90,
     EILSEQ: 92,
     EINPROGRESS: 36,
     EINTR: 4,
     EINVAL: 22,
     EIO: 5,
     EISCONN: 56,
     EISDIR: 21,
     ELOOP: 62,
     EMFILE: 24,
     EMLINK: 31,
     EMSGSIZE: 40,
     EMULTIHOP: 95,
     ENAMETOOLONG: 63,
     ENETDOWN: 50,
     ENETRESET: 52,
     ENETUNREACH: 51,
     ENFILE: 23,
     ENOBUFS: 55,
     ENODATA: 96,
     ENODEV: 19,
     ENOENT: 2,
     ENOEXEC: 8,
     ENOLCK: 77,
     ENOLINK: 97,
     ENOMEM: 12,
     ENOMSG: 91,
     ENOPROTOOPT: 42,
     ENOSPC: 28,
     ENOSR: 98,
     ENOSTR: 99,
     ENOSYS: 78,
     ENOTCONN: 57,
     ENOTDIR: 20,
     ENOTEMPTY: 66,
     ENOTSOCK: 38,
     ENOTSUP: 45,
     ENOTTY: 25,
     ENXIO: 6,
     EOPNOTSUPP: 102,
     EOVERFLOW: 84,
     EPERM: 1,
     EPIPE: 32,
     EPROTO: 100,
     EPROTONOSUPPORT: 43,
     EPROTOTYPE: 41,
     ERANGE: 34,
     EROFS: 30,
     ESPIPE: 29,
     ESRCH: 3,
     ESTALE: 70,
     ETIME: 101,
     ETIMEDOUT: 60,
     ETXTBSY: 26,
     EWOULDBLOCK: 35,
     EXDEV: 18 },
  signals:
   { SIGHUP: 1,
     SIGINT: 2,
     SIGQUIT: 3,
     SIGILL: 4,
     SIGTRAP: 5,
     SIGABRT: 6,
     SIGIOT: 6,
     SIGBUS: 10,
     SIGFPE: 8,
     SIGKILL: 9,
     SIGUSR1: 30,
     SIGSEGV: 11,
     SIGUSR2: 31,
     SIGPIPE: 13,
     SIGALRM: 14,
     SIGTERM: 15,
     SIGCHLD: 20,
     SIGCONT: 19,
     SIGSTOP: 17,
     SIGTSTP: 18,
     SIGTTIN: 21,
     SIGTTOU: 22,
     SIGURG: 16,
     SIGXCPU: 24,
     SIGXFSZ: 25,
     SIGVTALRM: 26,
     SIGPROF: 27,
     SIGWINCH: 28,
     SIGIO: 23,
     SIGINFO: 29,
     SIGSYS: 12 } }
```
