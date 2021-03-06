

#Module hackney_tcp_transport#
* [Function Index](#index)
* [Function Details](#functions)


<a name="index"></a>

##Function Index##


<table width="100%" border="1" cellspacing="0" cellpadding="2" summary="function index"><tr><td valign="top"><a href="#close-1">close/1</a></td><td>Close a TCP socket.</td></tr><tr><td valign="top"><a href="#connect-3">connect/3</a></td><td></td></tr><tr><td valign="top"><a href="#controlling_process-2">controlling_process/2</a></td><td>Assign a new controlling process <em>Pid</em> to <em>Socket</em>.</td></tr><tr><td valign="top"><a href="#peername-1">peername/1</a></td><td>Return the address and port for the other end of a connection.</td></tr><tr><td valign="top"><a href="#recv-2">recv/2</a></td><td></td></tr><tr><td valign="top"><a href="#recv-3">recv/3</a></td><td>Receive a packet from a socket in passive mode.</td></tr><tr><td valign="top"><a href="#send-2">send/2</a></td><td>Send a packet on a socket.</td></tr><tr><td valign="top"><a href="#setopts-2">setopts/2</a></td><td>Set one or more options for a socket.</td></tr><tr><td valign="top"><a href="#sockname-1">sockname/1</a></td><td>Get the local address and port of a socket.</td></tr></table>


<a name="functions"></a>

##Function Details##

<a name="close-1"></a>

###close/1##


<pre>close(Socket::<a href="inet.md#type-socket">inet:socket()</a>) -> ok</pre>
<br></br>


Close a TCP socket.

__See also:__ [gen_tcp:close/1](gen_tcp.md#close-1).<a name="connect-3"></a>

###connect/3##


`connect(Host, Port, Opts) -> any()`

<a name="controlling_process-2"></a>

###controlling_process/2##


<pre>controlling_process(Socket::<a href="inet.md#type-socket">inet:socket()</a>, Pid::pid()) -> ok | {error, closed | not_owner | atom()}</pre>
<br></br>


Assign a new controlling process _Pid_ to _Socket_.

__See also:__ [gen_tcp:controlling_process/2](gen_tcp.md#controlling_process-2).<a name="peername-1"></a>

###peername/1##


<pre>peername(Socket::<a href="inet.md#type-socket">inet:socket()</a>) -> {ok, {<a href="inet.md#type-ip_address">inet:ip_address()</a>, <a href="inet.md#type-port_number">inet:port_number()</a>}} | {error, atom()}</pre>
<br></br>


Return the address and port for the other end of a connection.

__See also:__ [inet:peername/1](inet.md#peername-1).<a name="recv-2"></a>

###recv/2##


`recv(Socket, Length) -> any()`

<a name="recv-3"></a>

###recv/3##


<pre>recv(Socket::<a href="inet.md#type-socket">inet:socket()</a>, Length::non_neg_integer(), Timeout::timeout()) -> {ok, any()} | {error, closed | atom()}</pre>
<br></br>


Receive a packet from a socket in passive mode.

__See also:__ [gen_tcp:recv/3](gen_tcp.md#recv-3).<a name="send-2"></a>

###send/2##


<pre>send(Socket::<a href="inet.md#type-socket">inet:socket()</a>, Packet::iolist()) -> ok | {error, atom()}</pre>
<br></br>


Send a packet on a socket.

__See also:__ [gen_tcp:send/2](gen_tcp.md#send-2).<a name="setopts-2"></a>

###setopts/2##


<pre>setopts(Socket::<a href="inet.md#type-socket">inet:socket()</a>, Opts::list()) -> ok | {error, atom()}</pre>
<br></br>


Set one or more options for a socket.

__See also:__ [inet:setopts/2](inet.md#setopts-2).<a name="sockname-1"></a>

###sockname/1##


<pre>sockname(Socket::<a href="inet.md#type-socket">inet:socket()</a>) -> {ok, {<a href="inet.md#type-ip_address">inet:ip_address()</a>, <a href="inet.md#type-port_number">inet:port_number()</a>}} | {error, atom()}</pre>
<br></br>


Get the local address and port of a socket

__See also:__ [inet:sockname/1](inet.md#sockname-1).