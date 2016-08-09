# random-vlc

class FileObject
{
system.filesystemobject o;

public void new(obj FOLDERLIST)
{
foreach folder in FOLDERLIST
{
	foreach file in folder
	{
		if file.typeinfo = "VLC MEDIA FILE" //HERE IS THE EDITTTTTTTTTTTTTTTTTTTTTTTTT
		{	
			o.adduri(file)
		}
	}
}
}

public void playRandom()
{
	int r = random(0, o.length())
	int c = 0
	foreach video in o
	{
		if c++ = r
		{
			EXEC vlc.exe o.uri
		}
	}
}
