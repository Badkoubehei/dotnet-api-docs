all: server.exe client.exe

server.exe: ChannelServices_registeredchannels_Server.cs ChannelServices_registeredchannels_Share.dll
	csc ChannelServices_registeredchannels_Server.cs /r:ChannelServices_registeredchannels_Share.dll

client.exe: channelservices_registeredchannels_client.cs ChannelServices_registeredchannels_Share.dll
	csc ChannelServices_registeredchannels_client.cs /r:ChannelServices_registeredchannels_Share.dll

ChannelServices_RegisteredChannels_Share.dll: ChannelServices_RegisteredChannels_Share.cs
	csc /t:library ChannelServices_RegisteredChannels_Share.cs
