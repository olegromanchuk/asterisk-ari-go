[![Go Reference](https://pkg.go.dev/badge/github.com/quintex-dev/asterisk-ari-go.svg)](https://pkg.go.dev/github.com/quintex-dev/asterisk-ari-go)

# Go API client Asterisk 18.13.0 LTS


Forked from `https://github.com/quintex-dev/asterisk-ari-go`



## Original documentation

This client is partly generated by [swagger-codegen](https://github.com/swagger-api/swagger-codegen) but also has gone 
through hand optimization and some manual changes to fit real world scenarios.

## Installation

Note: Please try to use the latest version of Go.

## Usage
After installation, simply import this package and start using it:
```
import "github.com/improcom/asterisk-ari-go"
```

## Documentation for API Endpoints

All URIs are relative to *http://xx.xx.xx.xx/ari* of your Asterisk server.

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ApplicationsApi* | [**Filter**](docs/ApplicationsApi.md#filter) | **Put** /applications/{applicationName}/eventFilter | Filter application events types.
*ApplicationsApi* | [**Get**](docs/ApplicationsApi.md#get) | **Get** /applications/{applicationName} | Get details of an application.
*ApplicationsApi* | [**List**](docs/ApplicationsApi.md#list) | **Get** /applications | List all applications.
*ApplicationsApi* | [**Subscribe**](docs/ApplicationsApi.md#subscribe) | **Post** /applications/{applicationName}/subscription | Subscribe an application to a event source.
*ApplicationsApi* | [**Unsubscribe**](docs/ApplicationsApi.md#unsubscribe) | **Delete** /applications/{applicationName}/subscription | Unsubscribe an application from an event source.
*AsteriskApi* | [**AddLog**](docs/AsteriskApi.md#addlog) | **Post** /asterisk/logging/{logChannelName} | Adds a log channel.
*AsteriskApi* | [**DeleteLog**](docs/AsteriskApi.md#deletelog) | **Delete** /asterisk/logging/{logChannelName} | Deletes a log channel.
*AsteriskApi* | [**DeleteObject**](docs/AsteriskApi.md#deleteobject) | **Delete** /asterisk/config/dynamic/{configClass}/{objectType}/{id} | Delete a dynamic configuration object.
*AsteriskApi* | [**GetGlobalVar**](docs/AsteriskApi.md#getglobalvar) | **Get** /asterisk/variable | Get the value of a global variable.
*AsteriskApi* | [**GetInfo**](docs/AsteriskApi.md#getinfo) | **Get** /asterisk/info | Gets Asterisk system information.
*AsteriskApi* | [**GetModule**](docs/AsteriskApi.md#getmodule) | **Get** /asterisk/modules/{moduleName} | Get Asterisk module information.
*AsteriskApi* | [**GetObject**](docs/AsteriskApi.md#getobject) | **Get** /asterisk/config/dynamic/{configClass}/{objectType}/{id} | Retrieve a dynamic configuration object.
*AsteriskApi* | [**ListLogChannels**](docs/AsteriskApi.md#listlogchannels) | **Get** /asterisk/logging | Gets Asterisk log channel information.
*AsteriskApi* | [**ListModules**](docs/AsteriskApi.md#listmodules) | **Get** /asterisk/modules | List Asterisk modules.
*AsteriskApi* | [**LoadModule**](docs/AsteriskApi.md#loadmodule) | **Post** /asterisk/modules/{moduleName} | Load an Asterisk module.
*AsteriskApi* | [**Ping**](docs/AsteriskApi.md#ping) | **Get** /asterisk/ping | Response pong message.
*AsteriskApi* | [**ReloadModule**](docs/AsteriskApi.md#reloadmodule) | **Put** /asterisk/modules/{moduleName} | Reload an Asterisk module.
*AsteriskApi* | [**RotateLog**](docs/AsteriskApi.md#rotatelog) | **Put** /asterisk/logging/{logChannelName}/rotate | Rotates a log channel.
*AsteriskApi* | [**SetGlobalVar**](docs/AsteriskApi.md#setglobalvar) | **Post** /asterisk/variable | Set the value of a global variable.
*AsteriskApi* | [**UnloadModule**](docs/AsteriskApi.md#unloadmodule) | **Delete** /asterisk/modules/{moduleName} | Unload an Asterisk module.
*AsteriskApi* | [**UpdateObject**](docs/AsteriskApi.md#updateobject) | **Put** /asterisk/config/dynamic/{configClass}/{objectType}/{id} | Create or update a dynamic configuration object.
*BridgesApi* | [**AddChannel**](docs/BridgesApi.md#addchannel) | **Post** /bridges/{bridgeId}/addChannel | Add a channel to a bridge.
*BridgesApi* | [**ClearVideoSource**](docs/BridgesApi.md#clearvideosource) | **Delete** /bridges/{bridgeId}/videoSource | Removes any explicit video source in a multi-party mixing bridge. This operation has no effect on bridges with two or fewer participants. When no explicit video source is set, talk detection will be used to determine the active video stream.
*BridgesApi* | [**Create**](docs/BridgesApi.md#create) | **Post** /bridges | Create a new bridge.
*BridgesApi* | [**CreateWithId**](docs/BridgesApi.md#createwithid) | **Post** /bridges/{bridgeId} | Create a new bridge or updates an existing one.
*BridgesApi* | [**Destroy**](docs/BridgesApi.md#destroy) | **Delete** /bridges/{bridgeId} | Shut down a bridge.
*BridgesApi* | [**Getbridge**](docs/BridgesApi.md#getbridge) | **Get** /bridges/{bridgeId} | Get bridge details.
*BridgesApi* | [**Listbridges**](docs/BridgesApi.md#listbridges) | **Get** /bridges | List all active bridges in Asterisk.
*BridgesApi* | [**Play**](docs/BridgesApi.md#play) | **Post** /bridges/{bridgeId}/play | Start playback of media on a bridge.
*BridgesApi* | [**PlayWithId**](docs/BridgesApi.md#playwithid) | **Post** /bridges/{bridgeId}/play/{playbackId} | Start playback of media on a bridge.
*BridgesApi* | [**Record**](docs/BridgesApi.md#record) | **Post** /bridges/{bridgeId}/record | Start a recording.
*BridgesApi* | [**RemoveChannel**](docs/BridgesApi.md#removechannel) | **Post** /bridges/{bridgeId}/removeChannel | Remove a channel from a bridge.
*BridgesApi* | [**SetVideoSource**](docs/BridgesApi.md#setvideosource) | **Post** /bridges/{bridgeId}/videoSource/{channelId} | Set a channel as the video source in a multi-party mixing bridge. This operation has no effect on bridges with two or fewer participants.
*BridgesApi* | [**StartMoh**](docs/BridgesApi.md#startmoh) | **Post** /bridges/{bridgeId}/moh | Play music on hold to a bridge or change the MOH class that is playing.
*BridgesApi* | [**StopMoh**](docs/BridgesApi.md#stopmoh) | **Delete** /bridges/{bridgeId}/moh | Stop playing music on hold to a bridge.
*ChannelsApi* | [**AddMoh**](docs/ChannelsApi.md#addmoh) | **Post** /channels/{channelId}/moh | Play music on hold to a channel.
*ChannelsApi* | [**Answer**](docs/ChannelsApi.md#answer) | **Post** /channels/{channelId}/answer | Answer a channel.
*ChannelsApi* | [**ContinueInDialplan**](docs/ChannelsApi.md#continueindialplan) | **Post** /channels/{channelId}/continue | Exit application; continue execution in the dialplan.
*ChannelsApi* | [**Createchannel**](docs/ChannelsApi.md#createchannel) | **Post** /channels/create | Create channel.
*ChannelsApi* | [**Deletemoh**](docs/ChannelsApi.md#deletemoh) | **Delete** /channels/{channelId}/moh | Stop playing music on hold to a channel.
*ChannelsApi* | [**Dial**](docs/ChannelsApi.md#dial) | **Post** /channels/{channelId}/dial | Dial a created channel.
*ChannelsApi* | [**ExternalMedia**](docs/ChannelsApi.md#externalmedia) | **Post** /channels/externalMedia | Start an External Media session.
*ChannelsApi* | [**GetChannelVar**](docs/ChannelsApi.md#getchannelvar) | **Get** /channels/{channelId}/variable | Get the value of a channel variable or function.
*ChannelsApi* | [**Getchannel**](docs/ChannelsApi.md#getchannel) | **Get** /channels/{channelId} | Channel details.
*ChannelsApi* | [**Hangup**](docs/ChannelsApi.md#hangup) | **Delete** /channels/{channelId} | Delete (i.e. hangup) a channel.
*ChannelsApi* | [**Hold**](docs/ChannelsApi.md#hold) | **Post** /channels/{channelId}/hold | Hold a channel.
*ChannelsApi* | [**Listchannels**](docs/ChannelsApi.md#listchannels) | **Get** /channels | List all active channels in Asterisk.
*ChannelsApi* | [**Move**](docs/ChannelsApi.md#move) | **Post** /channels/{channelId}/move | Move the channel from one Stasis application to another.
*ChannelsApi* | [**Mute**](docs/ChannelsApi.md#mute) | **Post** /channels/{channelId}/mute | Mute a channel.
*ChannelsApi* | [**Originate**](docs/ChannelsApi.md#originate) | **Post** /channels | Create a new channel (originate).
*ChannelsApi* | [**OriginateWithId**](docs/ChannelsApi.md#originatewithid) | **Post** /channels/{channelId} | Create a new channel (originate with id).
*ChannelsApi* | [**PlaySoundWithId**](docs/ChannelsApi.md#playsoundwithid) | **Post** /channels/{channelId}/play/{playbackId} | Start playback of media and specify the playbackId.
*ChannelsApi* | [**Playsound**](docs/ChannelsApi.md#playsound) | **Post** /channels/{channelId}/play | Start playback of media.
*ChannelsApi* | [**Recordchannel**](docs/ChannelsApi.md#recordchannel) | **Post** /channels/{channelId}/record | Start a recording.
*ChannelsApi* | [**Redirect**](docs/ChannelsApi.md#redirect) | **Post** /channels/{channelId}/redirect | Redirect the channel to a different location.
*ChannelsApi* | [**Ring**](docs/ChannelsApi.md#ring) | **Post** /channels/{channelId}/ring | Indicate ringing to a channel.
*ChannelsApi* | [**RingStop**](docs/ChannelsApi.md#ringstop) | **Delete** /channels/{channelId}/ring | Stop ringing indication on a channel if locally generated.
*ChannelsApi* | [**Rtpstatistics**](docs/ChannelsApi.md#rtpstatistics) | **Get** /channels/{channelId}/rtp_statistics | RTP stats on a channel.
*ChannelsApi* | [**SendDTMF**](docs/ChannelsApi.md#senddtmf) | **Post** /channels/{channelId}/dtmf | Send provided DTMF to a given channel.
*ChannelsApi* | [**SetChannelVar**](docs/ChannelsApi.md#setchannelvar) | **Post** /channels/{channelId}/variable | Set the value of a channel variable or function.
*ChannelsApi* | [**SnoopChannel**](docs/ChannelsApi.md#snoopchannel) | **Post** /channels/{channelId}/snoop | Start snooping.
*ChannelsApi* | [**SnoopChannelWithId**](docs/ChannelsApi.md#snoopchannelwithid) | **Post** /channels/{channelId}/snoop/{snoopId} | Start snooping.
*ChannelsApi* | [**StartSilence**](docs/ChannelsApi.md#startsilence) | **Post** /channels/{channelId}/silence | Play silence to a channel.
*ChannelsApi* | [**StopSilence**](docs/ChannelsApi.md#stopsilence) | **Delete** /channels/{channelId}/silence | Stop playing silence to a channel.
*ChannelsApi* | [**Unhold**](docs/ChannelsApi.md#unhold) | **Delete** /channels/{channelId}/hold | Remove a channel from hold.
*ChannelsApi* | [**Unmute**](docs/ChannelsApi.md#unmute) | **Delete** /channels/{channelId}/mute | Unmute a channel.
*DeviceStatesApi* | [**Delete**](docs/DeviceStatesApi.md#delete) | **Delete** /deviceStates/{deviceName} | Destroy a device-state controlled by ARI.
*DeviceStatesApi* | [**Getdevicestate**](docs/DeviceStatesApi.md#getdevicestate) | **Get** /deviceStates/{deviceName} | Retrieve the current state of a device.
*DeviceStatesApi* | [**ListDeviceStates**](docs/DeviceStatesApi.md#listdevicestates) | **Get** /deviceStates | List all ARI controlled device states.
*DeviceStatesApi* | [**Update**](docs/DeviceStatesApi.md#update) | **Put** /deviceStates/{deviceName} | Change the state of a device controlled by ARI. (Note - implicitly creates the device state).
*EndpointsApi* | [**Getendpoint**](docs/EndpointsApi.md#getendpoint) | **Get** /endpoints/{tech}/{resource} | Details for an endpoint.
*EndpointsApi* | [**ListByTech**](docs/EndpointsApi.md#listbytech) | **Get** /endpoints/{tech} | List available endoints for a given endpoint technology.
*EndpointsApi* | [**Listendpoints**](docs/EndpointsApi.md#listendpoints) | **Get** /endpoints | List all endpoints.
*EndpointsApi* | [**SendMessage**](docs/EndpointsApi.md#sendmessage) | **Put** /endpoints/sendMessage | Send a message to some technology URI or endpoint.
*EndpointsApi* | [**SendMessageToEndpoint**](docs/EndpointsApi.md#sendmessagetoendpoint) | **Put** /endpoints/{tech}/{resource}/sendMessage | Send a message to some endpoint in a technology.
*EventsApi* | [**EventWebsocket**](docs/EventsApi.md#eventwebsocket) | **Get** /events | WebSocket connection for events.
*EventsApi* | [**UserEvent**](docs/EventsApi.md#userevent) | **Post** /events/user/{eventName} | Generate a user event.
*MailboxesApi* | [**Deletemailbox**](docs/MailboxesApi.md#deletemailbox) | **Delete** /mailboxes/{mailboxName} | Destroy a mailbox.
*MailboxesApi* | [**Getmailbox**](docs/MailboxesApi.md#getmailbox) | **Get** /mailboxes/{mailboxName} | Retrieve the current state of a mailbox.
*MailboxesApi* | [**Listmailboxes**](docs/MailboxesApi.md#listmailboxes) | **Get** /mailboxes | List all mailboxes.
*MailboxesApi* | [**Updatemailbox**](docs/MailboxesApi.md#updatemailbox) | **Put** /mailboxes/{mailboxName} | Change the state of a mailbox. (Note - implicitly creates the mailbox).
*PlaybacksApi* | [**Control**](docs/PlaybacksApi.md#control) | **Post** /playbacks/{playbackId}/control | Control a playback.
*PlaybacksApi* | [**Getplayback**](docs/PlaybacksApi.md#getplayback) | **Get** /playbacks/{playbackId} | Get a playback&#39;s details.
*PlaybacksApi* | [**Stop**](docs/PlaybacksApi.md#stop) | **Delete** /playbacks/{playbackId} | Stop a playback.
*RecordingsApi* | [**Cancel**](docs/RecordingsApi.md#cancel) | **Delete** /recordings/live/{recordingName} | Stop a live recording and discard it.
*RecordingsApi* | [**CopyStored**](docs/RecordingsApi.md#copystored) | **Post** /recordings/stored/{recordingName}/copy | Copy a stored recording.
*RecordingsApi* | [**DeleteStored**](docs/RecordingsApi.md#deletestored) | **Delete** /recordings/stored/{recordingName} | Delete a stored recording.
*RecordingsApi* | [**GetLive**](docs/RecordingsApi.md#getlive) | **Get** /recordings/live/{recordingName} | List live recordings.
*RecordingsApi* | [**GetStored**](docs/RecordingsApi.md#getstored) | **Get** /recordings/stored/{recordingName} | Get a stored recording&#39;s details.
*RecordingsApi* | [**GetStoredFile**](docs/RecordingsApi.md#getstoredfile) | **Get** /recordings/stored/{recordingName}/file | Get the file associated with the stored recording.
*RecordingsApi* | [**ListStored**](docs/RecordingsApi.md#liststored) | **Get** /recordings/stored | List recordings that are complete.
*RecordingsApi* | [**Muterecording**](docs/RecordingsApi.md#muterecording) | **Post** /recordings/live/{recordingName}/mute | Mute a live recording.
*RecordingsApi* | [**Pause**](docs/RecordingsApi.md#pause) | **Post** /recordings/live/{recordingName}/pause | Pause a live recording.
*RecordingsApi* | [**Stoprecording**](docs/RecordingsApi.md#stoprecording) | **Post** /recordings/live/{recordingName}/stop | Stop a live recording and store it.
*RecordingsApi* | [**Unmuterecording**](docs/RecordingsApi.md#unmuterecording) | **Delete** /recordings/live/{recordingName}/mute | Unmute a live recording.
*RecordingsApi* | [**Unpause**](docs/RecordingsApi.md#unpause) | **Delete** /recordings/live/{recordingName}/pause | Unpause a live recording.
*SoundsApi* | [**Getsound**](docs/SoundsApi.md#getsound) | **Get** /sounds/{soundId} | Get a sound&#39;s details.
*SoundsApi* | [**Listsounds**](docs/SoundsApi.md#listsounds) | **Get** /sounds | List all sounds.


## Documentation For Models

 - [Application](docs/Application.md)
 - [ApplicationMoveFailed](docs/ApplicationMoveFailed.md)
 - [ApplicationReplaced](docs/ApplicationReplaced.md)
 - [AsteriskInfo](docs/AsteriskInfo.md)
 - [AsteriskPing](docs/AsteriskPing.md)
 - [Binary](docs/Binary.md)
 - [Bridge](docs/Bridge.md)
 - [BridgeAttendedTransfer](docs/BridgeAttendedTransfer.md)
 - [BridgeBlindTransfer](docs/BridgeBlindTransfer.md)
 - [BridgeCreated](docs/BridgeCreated.md)
 - [BridgeDestroyed](docs/BridgeDestroyed.md)
 - [BridgeMerged](docs/BridgeMerged.md)
 - [BridgeVideoSourceChanged](docs/BridgeVideoSourceChanged.md)
 - [BuildInfo](docs/BuildInfo.md)
 - [CallerId](docs/CallerId.md)
 - [Channel](docs/Channel.md)
 - [ChannelCallerId](docs/ChannelCallerId.md)
 - [ChannelConnectedLine](docs/ChannelConnectedLine.md)
 - [ChannelCreated](docs/ChannelCreated.md)
 - [ChannelDestroyed](docs/ChannelDestroyed.md)
 - [ChannelDialplan](docs/ChannelDialplan.md)
 - [ChannelDtmfReceived](docs/ChannelDtmfReceived.md)
 - [ChannelEnteredBridge](docs/ChannelEnteredBridge.md)
 - [ChannelHangupRequest](docs/ChannelHangupRequest.md)
 - [ChannelHold](docs/ChannelHold.md)
 - [ChannelLeftBridge](docs/ChannelLeftBridge.md)
 - [ChannelStateChange](docs/ChannelStateChange.md)
 - [ChannelTalkingFinished](docs/ChannelTalkingFinished.md)
 - [ChannelTalkingStarted](docs/ChannelTalkingStarted.md)
 - [ChannelUnhold](docs/ChannelUnhold.md)
 - [ChannelUserevent](docs/ChannelUserevent.md)
 - [ChannelVarset](docs/ChannelVarset.md)
 - [ConfigInfo](docs/ConfigInfo.md)
 - [ConfigTuple](docs/ConfigTuple.md)
 - [ContactInfo](docs/ContactInfo.md)
 - [ContactStatusChange](docs/ContactStatusChange.md)
 - [Containers](docs/Containers.md)
 - [DeviceState](docs/DeviceState.md)
 - [DeviceStateChanged](docs/DeviceStateChanged.md)
 - [Dial](docs/Dial.md)
 - [Dialed](docs/Dialed.md)
 - [DialplanCep](docs/DialplanCep.md)
 - [Endpoint](docs/Endpoint.md)
 - [EndpointStateChange](docs/EndpointStateChange.md)
 - [Event](docs/Event.md)
 - [FormatLangPair](docs/FormatLangPair.md)
 - [LiveRecording](docs/LiveRecording.md)
 - [LogChannel](docs/LogChannel.md)
 - [Mailbox](docs/Mailbox.md)
 - [Message](docs/Message.md)
 - [MissingParams](docs/MissingParams.md)
 - [Module](docs/Module.md)
 - [Peer](docs/Peer.md)
 - [PeerStatusChange](docs/PeerStatusChange.md)
 - [Playback](docs/Playback.md)
 - [PlaybackContinuing](docs/PlaybackContinuing.md)
 - [PlaybackFinished](docs/PlaybackFinished.md)
 - [PlaybackStarted](docs/PlaybackStarted.md)
 - [RecordingFailed](docs/RecordingFailed.md)
 - [RecordingFinished](docs/RecordingFinished.md)
 - [RecordingStarted](docs/RecordingStarted.md)
 - [RtPstat](docs/RtPstat.md)
 - [SetId](docs/SetId.md)
 - [Sound](docs/Sound.md)
 - [StasisEnd](docs/StasisEnd.md)
 - [StasisStart](docs/StasisStart.md)
 - [StatusInfo](docs/StatusInfo.md)
 - [StoredRecording](docs/StoredRecording.md)
 - [SystemInfo](docs/SystemInfo.md)
 - [TextMessage](docs/TextMessage.md)
 - [TextMessageReceived](docs/TextMessageReceived.md)
 - [Variable](docs/Variable.md)


## Documentation For Authorization
 Asterisk ARI uses HTTP Basic Authorization. ``Go context.Context`` is used to pass in the HTTP Basic Authorization 
 credentials.

## Author
Chris Roy [@chris](https://twitter.com/@chrisroy87) <br />
With love from - **Quintex Software Solutions Pvt. Ltd.**

