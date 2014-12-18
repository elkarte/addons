{% capture osi %}{{ include.param | upcase | remove: '-' | remove: ' ' | remove: '.' | remove: 'V' | truncate: 5, '' }}{% endcapture %}

{% case osi %}
	{% when 'BSD' or 'BSD3' %}
This ElkArte Addon is subject to the terms of the BSD 3-Clause Simplified (the "License"). You can obtain a copy of the License at http://opensource.org/licenses/BSD-3-Clause
	{% when 'BSD2' %}
This ElkArte Addon is subject to the terms of the The BSD 2-Clause License (the "License"). You can obtain a copy of the License at http://opensource.org/licenses/BSD-2-Clause
	{% when 'MPL11' %}
This ElkArte Addon is subject to the terms of the Mozilla Public License version 1.1 (the "License"). You can obtain a copy of the License at https://www.mozilla.org/MPL/1.1/
	{% when 'MPL' or 'MPL20' %}
This ElkArte Addon is subject to the terms of the Mozilla Public License version 2 (the "License"). You can obtain a copy of the License at https://www.mozilla.org/MPL/2.0/
	{% when 'GNU20' or 'GPL20' %}
This ElkArte Addon is subject to the terms of the GNU General Public License, version 2 (the "License"). You can obtain a copy of the License at http://opensource.org/licenses/GPL-2.0
	{% when 'GNU3' or 'GPL3' or 'GPL' %}
This ElkArte Addon is subject to the terms of the GNU General Public License, version 3 (the "License"). You can obtain a copy of the License at http://opensource.org/licenses/GPL-3.0
	{% when 'APACH' %}
This ElkArte Addon is subject to the terms of the Apache License, Version 2.0 (the "License"). You can obtain a copy of the License at http://opensource.org/licenses/Apache-2.0
	{% when 'LGPL3' or 'LGPL' %}
This ElkArte Addon is subject to the terms of the GNU Lesser General Public License, version 3.0 (LGPL-3.0) (the "License"). You can obtain a copy of the License at http://opensource.org/licenses/LGPL-3.0
	{% when 'WTF' or 'WTF10' %}
This ElkArte Addon is subject to the terms of the he WTF General Public License, version 1.0 (WTF-1.0) (the "License"). You can obtain a copy of the License at http://www.wtfpl.net/txt/copying/
	{% when 'MIT' %}
This ElkArte Addon is subject to the terms of the The MIT License (MIT)  (the "License"). You can obtain a copy of the License at http://opensource.org/licenses/MIT
	{% else %}
Unknown
{% endcase %}