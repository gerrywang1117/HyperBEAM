# [Module dev_push.erl](https://github.com/permaweb/HyperBEAM/blob/main/src/dev_push.erl)




`push@1.0` takes a message or slot number, evaluates it, and recursively
pushes the resulting messages to other processes.

<a name="description"></a>

## Description ##
The `push`ing mechanism
continues until the there are no remaining messages to push.<a name="index"></a>

## Function Index ##


<table width="100%" border="1" cellspacing="0" cellpadding="2" summary="function index"><tr><td valign="top"><a href="#additional_keys-3">additional_keys/3*</a></td><td>Set the necessary keys in order for the recipient to know where the
message came from.</td></tr><tr><td valign="top"><a href="#do_push-3">do_push/3*</a></td><td>Push a message or slot number.</td></tr><tr><td valign="top"><a href="#extract-2">extract/2*</a></td><td>Return either the <code>target</code> or the <code>hint</code>.</td></tr><tr><td valign="top"><a href="#find_type-2">find_type/2*</a></td><td></td></tr><tr><td valign="top"><a href="#full_push_test_-0">full_push_test_/0*</a></td><td></td></tr><tr><td valign="top"><a href="#is_async-3">is_async/3*</a></td><td>Determine if the push is asynchronous.</td></tr><tr><td valign="top"><a href="#multi_process_push_test_disabled-0">multi_process_push_test_disabled/0*</a></td><td></td></tr><tr><td valign="top"><a href="#normalize_message-2">normalize_message/2*</a></td><td>Augment the message with from-* keys, if it doesn't already have them.</td></tr><tr><td valign="top"><a href="#parse_redirect-1">parse_redirect/1*</a></td><td></td></tr><tr><td valign="top"><a href="#ping_pong_script-1">ping_pong_script/1*</a></td><td></td></tr><tr><td valign="top"><a href="#push-3">push/3</a></td><td>Push either a message or an assigned slot number.</td></tr><tr><td valign="top"><a href="#push_prompts_encoding_change_test-0">push_prompts_encoding_change_test/0*</a></td><td></td></tr><tr><td valign="top"><a href="#push_result_message-5">push_result_message/5*</a></td><td></td></tr><tr><td valign="top"><a href="#push_with_mode-3">push_with_mode/3*</a></td><td></td></tr><tr><td valign="top"><a href="#push_with_redirect_hint_test_disabled-0">push_with_redirect_hint_test_disabled/0*</a></td><td></td></tr><tr><td valign="top"><a href="#remote_schedule_result-3">remote_schedule_result/3*</a></td><td></td></tr><tr><td valign="top"><a href="#reply_script-0">reply_script/0*</a></td><td></td></tr><tr><td valign="top"><a href="#schedule_initial_message-3">schedule_initial_message/3*</a></td><td>Push a message or a process, prior to pushing the resulting slot number.</td></tr><tr><td valign="top"><a href="#schedule_result-3">schedule_result/3*</a></td><td></td></tr><tr><td valign="top"><a href="#schedule_result-4">schedule_result/4*</a></td><td></td></tr><tr><td valign="top"><a href="#split_target-1">split_target/1*</a></td><td></td></tr><tr><td valign="top"><a href="#target_process-2">target_process/2*</a></td><td>Find the target process ID for a message to push.</td></tr></table>


<a name="functions"></a>

## Function Details ##

<a name="additional_keys-3"></a>

### additional_keys/3 * ###

`additional_keys(FromMsg, ToSched, Opts) -> any()`

Set the necessary keys in order for the recipient to know where the
message came from.

<a name="do_push-3"></a>

### do_push/3 * ###

`do_push(Base, Assignment, Opts) -> any()`

Push a message or slot number.

<a name="extract-2"></a>

### extract/2 * ###

`extract(X1, Raw) -> any()`

Return either the `target` or the `hint`.

<a name="find_type-2"></a>

### find_type/2 * ###

`find_type(Req, Opts) -> any()`

<a name="full_push_test_-0"></a>

### full_push_test_/0 * ###

`full_push_test_() -> any()`

<a name="is_async-3"></a>

### is_async/3 * ###

`is_async(Base, Req, Opts) -> any()`

Determine if the push is asynchronous.

<a name="multi_process_push_test_disabled-0"></a>

### multi_process_push_test_disabled/0 * ###

`multi_process_push_test_disabled() -> any()`

<a name="normalize_message-2"></a>

### normalize_message/2 * ###

`normalize_message(MsgToPush, Opts) -> any()`

Augment the message with from-* keys, if it doesn't already have them.

<a name="parse_redirect-1"></a>

### parse_redirect/1 * ###

`parse_redirect(Location) -> any()`

<a name="ping_pong_script-1"></a>

### ping_pong_script/1 * ###

`ping_pong_script(Limit) -> any()`

<a name="push-3"></a>

### push/3 ###

`push(Base, Req, Opts) -> any()`

Push either a message or an assigned slot number.

<a name="push_prompts_encoding_change_test-0"></a>

### push_prompts_encoding_change_test/0 * ###

`push_prompts_encoding_change_test() -> any()`

<a name="push_result_message-5"></a>

### push_result_message/5 * ###

`push_result_message(Base, FromSlot, Key, MsgToPush, Opts) -> any()`

<a name="push_with_mode-3"></a>

### push_with_mode/3 * ###

`push_with_mode(Base, Req, Opts) -> any()`

<a name="push_with_redirect_hint_test_disabled-0"></a>

### push_with_redirect_hint_test_disabled/0 * ###

`push_with_redirect_hint_test_disabled() -> any()`

<a name="remote_schedule_result-3"></a>

### remote_schedule_result/3 * ###

`remote_schedule_result(Location, SignedReq, Opts) -> any()`

<a name="reply_script-0"></a>

### reply_script/0 * ###

`reply_script() -> any()`

<a name="schedule_initial_message-3"></a>

### schedule_initial_message/3 * ###

`schedule_initial_message(Base, Req, Opts) -> any()`

Push a message or a process, prior to pushing the resulting slot number.

<a name="schedule_result-3"></a>

### schedule_result/3 * ###

`schedule_result(Base, MsgToPush, Opts) -> any()`

<a name="schedule_result-4"></a>

### schedule_result/4 * ###

`schedule_result(Base, MsgToPush, Codec, Opts) -> any()`

<a name="split_target-1"></a>

### split_target/1 * ###

`split_target(RawTarget) -> any()`

<a name="target_process-2"></a>

### target_process/2 * ###

`target_process(MsgToPush, Opts) -> any()`

Find the target process ID for a message to push.

