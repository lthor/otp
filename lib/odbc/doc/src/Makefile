#
# %CopyrightBegin%
#
# Copyright Ericsson AB 1999-2024. All Rights Reserved.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
# %CopyrightEnd%
#

#
include $(ERL_TOP)/make/target.mk
include $(ERL_TOP)/make/$(TARGET)/otp.mk

# ----------------------------------------------------
# Application version
# ----------------------------------------------------
include ../../vsn.mk
VSN=$(ODBC_VSN)
APPLICATION=odbc

# ----------------------------------------------------
# Target Specs
# ----------------------------------------------------
XML_APPLICATION_FILES = ref_man.xml
XML_REF3_FILES = odbc.xml

XML_PART_FILES = part.xml

XML_HTML_FILES = \
	notes_history.xml

XML_CHAPTER_FILES = \
	introduction.xml \
	getting_started.xml \
	databases.xml \
	error_handling.xml \
	notes.xml

BOOK_FILES = book.xml

XML_FILES = $(BOOK_FILES) $(XML_APPLICATION_FILES) $(XML_REF3_FILES) \
            $(XML_PART_FILES) $(XML_CHAPTER_FILES)

SPECS_FILES = $(XML_REF3_FILES:%.xml=$(SPECDIR)/specs_%.xml)

TOP_SPECS_FILE = specs.xml

IMAGE_FILES = \
	odbc_app_arc.gif

# ----------------------------------------------------
include $(ERL_TOP)/make/doc.mk
