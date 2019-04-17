# cpm
CPM - Control Process Memory

This simple tool leverages Linux CGROUPS (control groups) to limit process (and its children) memory utilization.

# Install

After downloading cpm executable (bash script), make it executable and copy e.g. to /usr/local/bin directory.

		cp cpm /usr/local/bin/
		chmod 755 /usr/local/bin/cpm

# Syntax

Limit sosreport process (with option --batch) and its children to 300 MiB of RAM. If parent process or any of its children attempts to use more RAM, it will get killed.

		cpm 300 sosreport --batch

