nanosvg for C#
===

## Overview
This is a line-by-line port of the [nanosvg](https://code.google.com/p/nanosvg/) parsing library, from C to C#. All file IO related methods have been removed.

##Usage

	// Load
	string svgData = ...;
	SvgPath plist = SvgParser.SvgParse(svgData);
	
	// Use...
	for (SvgPath it = plist; it != null; it = it.next)
		... // Draw stuff here
		
## License

	Copyright (c) 2009 Mikko Mononen memon@inside.org
	Ported to C# 2013 by Thinksquirrel Software, LLC

	This software is provided 'as-is', without any express or implied
	warranty.  In no event will the authors be held liable for any damages
	arising from the use of this software.
	Permission is granted to anyone to use this software for any purpose,
	including commercial applications, and to alter it and redistribute it
	freely, subject to the following restrictions:
	1. The origin of this software must not be misrepresented; you must not
	claim that you wrote the original software. If you use this software
	in a product, an acknowledgment in the product documentation would be
	appreciated but is not required.
	2. Altered source versions must be plainly marked as such, and must not be
	misrepresented as being the original software.
	3. This notice may not be removed or altered from any source distribution.

	The SVG parser is based on Anti-Graim Geometry SVG example
	Copyright (C) 2002-2004 Maxim Shemanarev (McSeem)