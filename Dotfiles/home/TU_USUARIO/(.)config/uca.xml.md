```
<?xml version="1.0" encoding="UTF-8"?>
<actions>
<action>
	<icon>utilities-terminal</icon>
	<name>Abrir Terminal aquí</name>
	<submenu></submenu>
	<unique-id>1778551402721842-1</unique-id>
	<command>exo-open --working-directory %f --launch TerminalEmulator</command>
	<description>Ejecutar la Terminal en el directorio</description>
	<range></range>
	<patterns>*</patterns>
	<startup-notify/>
	<directories/>
</action>
<action>
	<icon>edit-delete</icon>
	<name>Eliminar de forma segura</name>
	<submenu></submenu>
	<unique-id>1780094767826021-1</unique-id>
	<command>srm -r %F</command>
	<description>Sobreescribir archivos y carpetas</description>
	<range>*</range>
	<patterns>*</patterns>
	<directories/>
	<audio-files/>
	<image-files/>
	<other-files/>
	<text-files/>
	<video-files/>
</action>
</actions>
```