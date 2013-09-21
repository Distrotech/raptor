# -*- Mode: Makefile -*-
#
# Makefile.am - automake file for Raptor TriG 2013 tests
#
# Copyright (C) 2013, David Beckett http://www.dajobe.org/
# 
# This package is Free Software and part of Redland http://librdf.org/
# 
# It is licensed under the following three licenses as alternatives:
#   1. GNU Lesser General Public License (LGPL) V2.1 or any newer version
#   2. GNU General Public License (GPL) V2 or any newer version
#   3. Apache License, V2.0 or any newer version
# 
# You may not use this file except in compliance with at least one of
# the above three licenses.
# 
# See LICENSE.html or LICENSE.txt at the top of this package for the
# complete terms and further detail along with the license texts for
# the licenses in COPYING.LIB, COPYING and LICENSE-2.0.txt respectively.
# 
# 

RDFCOMPARE=$(srcdir)/../../scripts/rdfcompare

RDFXML_DIR = ../rdfxml
NTRIPLES_DIR = ../ntriples

# Good: http://www.w3.org/ns/rdftest#TestTrigPositiveSyntax
TEST_GOOD_FILES = \
  trig-kw-graph-01.trig \
  trig-kw-graph-02.trig \
  trig-kw-graph-03.trig \
  trig-kw-graph-04.trig \
  trig-kw-graph-05.trig \
  trig-kw-graph-06.trig \
  trig-kw-graph-07.trig \
  trig-kw-graph-08.trig \
  trig-kw-graph-09.trig \
  trig-kw-graph-10.trig \
  trig-syntax-base-01.trig \
  trig-syntax-base-02.trig \
  trig-syntax-base-03.trig \
  trig-syntax-base-04.trig \
  trig-syntax-blank-label.trig \
  trig-syntax-bnode-01.trig \
  trig-syntax-bnode-02.trig \
  trig-syntax-bnode-03.trig \
  trig-syntax-bnode-04.trig \
  trig-syntax-bnode-05.trig \
  trig-syntax-bnode-06.trig \
  trig-syntax-bnode-07.trig \
  trig-syntax-bnode-08.trig \
  trig-syntax-bnode-09.trig \
  trig-syntax-bnode-10.trig \
  trig-syntax-datatypes-01.trig \
  trig-syntax-datatypes-02.trig \
  trig-syntax-file-01.trig \
  trig-syntax-file-02.trig \
  trig-syntax-file-03.trig \
  trig-syntax-kw-01.trig \
  trig-syntax-kw-02.trig \
  trig-syntax-kw-03.trig \
  trig-syntax-lists-01.trig \
  trig-syntax-lists-02.trig \
  trig-syntax-lists-03.trig \
  trig-syntax-lists-04.trig \
  trig-syntax-lists-05.trig \
  trig-syntax-ln-colons.trig \
  trig-syntax-ln-dots.trig \
  trig-syntax-ns-dots.trig \
  trig-syntax-number-01.trig \
  trig-syntax-number-02.trig \
  trig-syntax-number-03.trig \
  trig-syntax-number-04.trig \
  trig-syntax-number-05.trig \
  trig-syntax-number-06.trig \
  trig-syntax-number-07.trig \
  trig-syntax-number-08.trig \
  trig-syntax-number-09.trig \
  trig-syntax-number-10.trig \
  trig-syntax-number-11.trig \
  trig-syntax-pname-esc-01.trig \
  trig-syntax-pname-esc-02.trig \
  trig-syntax-pname-esc-03.trig \
  trig-syntax-prefix-01.trig \
  trig-syntax-prefix-02.trig \
  trig-syntax-prefix-03.trig \
  trig-syntax-prefix-04.trig \
  trig-syntax-prefix-05.trig \
  trig-syntax-prefix-06.trig \
  trig-syntax-prefix-07.trig \
  trig-syntax-prefix-08.trig \
  trig-syntax-prefix-09.trig \
  trig-syntax-str-esc-01.trig \
  trig-syntax-str-esc-02.trig \
  trig-syntax-str-esc-03.trig \
  trig-syntax-string-01.trig \
  trig-syntax-string-02.trig \
  trig-syntax-string-03.trig \
  trig-syntax-string-04.trig \
  trig-syntax-string-05.trig \
  trig-syntax-string-06.trig \
  trig-syntax-string-07.trig \
  trig-syntax-string-08.trig \
  trig-syntax-string-09.trig \
  trig-syntax-string-10.trig \
  trig-syntax-string-11.trig \
  trig-syntax-struct-01.trig \
  trig-syntax-struct-02.trig \
  trig-syntax-struct-03.trig \
  trig-syntax-struct-04.trig \
  trig-syntax-struct-05.trig \
  trig-syntax-struct-06.trig \
  trig-syntax-struct-07.trig \
  trig-syntax-uri-01.trig \
  trig-syntax-uri-02.trig \
  trig-syntax-uri-03.trig \
  trig-syntax-uri-04.trig \
  trig-turtle-01.trig \
  trig-turtle-02.trig \
  trig-turtle-03.trig \
  trig-turtle-04.trig \
  trig-turtle-05.trig \
  trig-turtle-06.trig

# Bad: http://www.w3.org/ns/rdftest#TestTrigNegativeSyntax
TEST_BAD_FILES = \
  trig-bnodeplist-graph-bad-01.trig \
  trig-collection-graph-bad-01.trig \
  trig-collection-graph-bad-02.trig \
  trig-graph-bad-01.trig \
  trig-graph-bad-02.trig \
  trig-graph-bad-03.trig \
  trig-graph-bad-04.trig \
  trig-graph-bad-05.trig \
  trig-graph-bad-06.trig \
  trig-graph-bad-07.trig \
  trig-graph-bad-08.trig \
  trig-graph-bad-09.trig \
  trig-graph-bad-10.trig \
  trig-graph-bad-11.trig \
  trig-syntax-bad-LITERAL2_with_langtag_and_datatype.trig \
  trig-syntax-bad-base-01.trig \
  trig-syntax-bad-base-02.trig \
  trig-syntax-bad-base-03.trig \
  trig-syntax-bad-base-04.trig \
  trig-syntax-bad-base-05.trig \
  trig-syntax-bad-blank-label-dot-end.trig \
  trig-syntax-bad-esc-01.trig \
  trig-syntax-bad-esc-02.trig \
  trig-syntax-bad-esc-03.trig \
  trig-syntax-bad-esc-04.trig \
  trig-syntax-bad-kw-01.trig \
  trig-syntax-bad-kw-02.trig \
  trig-syntax-bad-kw-03.trig \
  trig-syntax-bad-kw-04.trig \
  trig-syntax-bad-kw-05.trig \
  trig-syntax-bad-lang-01.trig \
  trig-syntax-bad-ln-dash-start.trig \
  trig-syntax-bad-ln-escape-start.trig \
  trig-syntax-bad-ln-escape.trig \
  trig-syntax-bad-missing-ns-dot-end.trig \
  trig-syntax-bad-missing-ns-dot-start.trig \
  trig-syntax-bad-n3-extras-01.trig \
  trig-syntax-bad-n3-extras-02.trig \
  trig-syntax-bad-n3-extras-03.trig \
  trig-syntax-bad-n3-extras-04.trig \
  trig-syntax-bad-n3-extras-05.trig \
  trig-syntax-bad-n3-extras-06.trig \
  trig-syntax-bad-n3-extras-07.trig \
  trig-syntax-bad-n3-extras-08.trig \
  trig-syntax-bad-n3-extras-09.trig \
  trig-syntax-bad-n3-extras-10.trig \
  trig-syntax-bad-n3-extras-11.trig \
  trig-syntax-bad-n3-extras-12.trig \
  trig-syntax-bad-n3-extras-13.trig \
  trig-syntax-bad-ns-dot-end.trig \
  trig-syntax-bad-ns-dot-start.trig \
  trig-syntax-bad-num-01.trig \
  trig-syntax-bad-num-02.trig \
  trig-syntax-bad-num-03.trig \
  trig-syntax-bad-num-04.trig \
  trig-syntax-bad-num-05.trig \
  trig-syntax-bad-number-dot-in-anon.trig \
  trig-syntax-bad-pname-01.trig \
  trig-syntax-bad-pname-02.trig \
  trig-syntax-bad-pname-03.trig \
  trig-syntax-bad-prefix-01.trig \
  trig-syntax-bad-prefix-02.trig \
  trig-syntax-bad-prefix-03.trig \
  trig-syntax-bad-prefix-04.trig \
  trig-syntax-bad-prefix-05.trig \
  trig-syntax-bad-prefix-06.trig \
  trig-syntax-bad-prefix-07.trig \
  trig-syntax-bad-string-01.trig \
  trig-syntax-bad-string-02.trig \
  trig-syntax-bad-string-03.trig \
  trig-syntax-bad-string-04.trig \
  trig-syntax-bad-string-05.trig \
  trig-syntax-bad-string-06.trig \
  trig-syntax-bad-string-07.trig \
  trig-syntax-bad-struct-02.trig \
  trig-syntax-bad-struct-03.trig \
  trig-syntax-bad-struct-04.trig \
  trig-syntax-bad-struct-05.trig \
  trig-syntax-bad-struct-06.trig \
  trig-syntax-bad-struct-07.trig \
  trig-syntax-bad-struct-09.trig \
  trig-syntax-bad-struct-10.trig \
  trig-syntax-bad-struct-12.trig \
  trig-syntax-bad-struct-13.trig \
  trig-syntax-bad-struct-14.trig \
  trig-syntax-bad-struct-15.trig \
  trig-syntax-bad-struct-16.trig \
  trig-syntax-bad-struct-17.trig \
  trig-syntax-bad-uri-01.trig \
  trig-syntax-bad-uri-02.trig \
  trig-syntax-bad-uri-03.trig \
  trig-syntax-bad-uri-04.trig \
  trig-syntax-bad-uri-05.trig \
  trig-turtle-bad-01.trig \
  trig-turtle-bad-02.trig

# Good: http://www.w3.org/ns/rdftest#TestTrigEval
TEST_EVAL_FILES = \
  HYPHEN_MINUS_in_localName.trig \
  IRIREF_datatype.trig \
  IRI_subject.trig \
  IRI_with_all_punctuation.trig \
  IRI_with_eight_digit_numeric_escape.trig \
  IRI_with_four_digit_numeric_escape.trig \
  LITERAL1.trig \
  LITERAL1_all_controls.trig \
  LITERAL1_all_punctuation.trig \
  LITERAL1_ascii_boundaries.trig \
  LITERAL2.trig \
  LITERAL2_ascii_boundaries.trig \
  LITERAL_LONG1.trig \
  LITERAL_LONG1_ascii_boundaries.trig \
  LITERAL_LONG1_with_1_squote.trig \
  LITERAL_LONG1_with_2_squotes.trig \
  LITERAL_LONG2.trig \
  LITERAL_LONG2_ascii_boundaries.trig \
  LITERAL_LONG2_with_1_squote.trig \
  LITERAL_LONG2_with_2_squotes.trig \
  LITERAL_LONG2_with_REVERSE_SOLIDUS.trig \
  SPARQL_style_base.trig \
  SPARQL_style_prefix.trig \
  alternating_bnode_graphs.trig \
  alternating_iri_graphs.trig \
  anonymous_blank_node_graph.trig \
  anonymous_blank_node_object.trig \
  anonymous_blank_node_subject.trig \
  bareword_a_predicate.trig \
  bareword_decimal.trig \
  bareword_double.trig \
  bareword_integer.trig \
  blankNodePropertyList_as_object.trig \
  blankNodePropertyList_as_subject.trig \
  blankNodePropertyList_containing_collection.trig \
  blankNodePropertyList_with_multiple_triples.trig \
  collection_object.trig \
  collection_subject.trig \
  default_namespace_IRI.trig \
  double_lower_case_e.trig \
  empty_collection.trig \
  first.trig \
  labeled_blank_node_graph.trig \
  labeled_blank_node_object.trig \
  labeled_blank_node_subject.trig \
  labeled_blank_node_with_PN_CHARS_BASE_char_boundaries.trig \
  labeled_blank_node_with_leading_digit.trig \
  labeled_blank_node_with_leading_underscore.trig \
  labeled_blank_node_with_non_leading_extras.trig \
  langtagged_LONG.trig \
  langtagged_LONG_with_subtag.trig \
  langtagged_non_LONG.trig \
  lantag_with_subtag.trig \
  last.trig \
  literal_false.trig \
  literal_true.trig \
  literal_with_BACKSPACE.trig \
  literal_with_CARRIAGE_RETURN.trig \
  literal_with_CHARACTER_TABULATION.trig \
  literal_with_FORM_FEED.trig \
  literal_with_LINE_FEED.trig \
  literal_with_REVERSE_SOLIDUS.trig \
  literal_with_escaped_BACKSPACE.trig \
  literal_with_escaped_CARRIAGE_RETURN.trig \
  literal_with_escaped_CHARACTER_TABULATION.trig \
  literal_with_escaped_FORM_FEED.trig \
  literal_with_escaped_LINE_FEED.trig \
  literal_with_numeric_escape4.trig \
  literal_with_numeric_escape8.trig \
  localName_with_PN_CHARS_BASE_char_boundaries.trig \
  localName_with_assigned_nfc_PN_CHARS_BASE_char_boundaries.trig \
  localName_with_assigned_nfc_bmp_PN_CHARS_BASE_char_boundaries.trig \
  localName_with_leading_digit.trig \
  localName_with_leading_underscore.trig \
  localName_with_nfc_PN_CHARS_BASE_char_boundaries.trig \
  localName_with_non_leading_extras.trig \
  localname_with_COLON.trig \
  negative_numeric.trig \
  nested_blankNodePropertyLists.trig \
  nested_collection.trig \
  numeric_with_leading_0.trig \
  objectList_with_two_objects.trig \
  old_style_base.trig \
  old_style_prefix.trig \
  percent_escaped_localName.trig \
  positive_numeric.trig \
  predicateObjectList_with_two_objectLists.trig \
  prefix_only_IRI.trig \
  prefix_reassigned_and_used.trig \
  prefix_with_PN_CHARS_BASE_char_boundaries.trig \
  prefix_with_non_leading_extras.trig \
  prefixed_IRI_object.trig \
  prefixed_IRI_predicate.trig \
  prefixed_name_datatype.trig \
  repeated_semis_at_end.trig \
  repeated_semis_not_at_end.trig \
  reserved_escaped_localName.trig \
  sole_blankNodePropertyList.trig \
  trig-eval-struct-01.trig \
  trig-eval-struct-02.trig \
  trig-subm-01.trig \
  trig-subm-02.trig \
  trig-subm-03.trig \
  trig-subm-04.trig \
  trig-subm-05.trig \
  trig-subm-06.trig \
  trig-subm-07.trig \
  trig-subm-08.trig \
  trig-subm-09.trig \
  trig-subm-10.trig \
  trig-subm-11.trig \
  trig-subm-12.trig \
  trig-subm-13.trig \
  trig-subm-14.trig \
  trig-subm-15.trig \
  trig-subm-16.trig \
  trig-subm-17.trig \
  trig-subm-18.trig \
  trig-subm-19.trig \
  trig-subm-20.trig \
  trig-subm-21.trig \
  trig-subm-22.trig \
  trig-subm-23.trig \
  trig-subm-24.trig \
  trig-subm-25.trig \
  trig-subm-26.trig \
  trig-subm-27.trig \
  two_LITERAL_LONG2s.trig \
  underscore_in_localName.trig

# Bad http://www.w3.org/ns/rdftest#TestTrigNegativeEval
TEST_BAD_EVAL_FILES = \
  trig-eval-bad-01.trig \
  trig-eval-bad-02.trig \
  trig-eval-bad-03.trig \
  trig-eval-bad-04.trig

TEST_OUT_FILES = \
  HYPHEN_MINUS_in_localName.nq \
  IRIREF_datatype.nq \
  IRI_spo.nq \
  IRI_with_all_punctuation.nq \
  LITERAL1.nq \
  LITERAL1_all_controls.nq \
  LITERAL1_all_punctuation.nq \
  LITERAL1_ascii_boundaries.nq \
  LITERAL2_ascii_boundaries.nq \
  LITERAL_LONG1_ascii_boundaries.nq \
  LITERAL_LONG1_with_1_squote.nq \
  LITERAL_LONG1_with_2_squotes.nq \
  LITERAL_LONG2_ascii_boundaries.nq \
  LITERAL_LONG2_with_1_squote.nq \
  LITERAL_LONG2_with_2_squotes.nq \
  LITERAL_LONG2_with_REVERSE_SOLIDUS.nq \
  alternating_bnode_graphs.nq \
  alternating_iri_graphs.nq \
  anonymous_blank_node_object.nq \
  anonymous_blank_node_subject.nq \
  bareword_a_predicate.nq \
  bareword_decimal.nq \
  bareword_double.nq \
  blankNodePropertyList_as_object.nq \
  blankNodePropertyList_as_subject.nq \
  blankNodePropertyList_containing_collection.nq \
  blankNodePropertyList_with_multiple_triples.nq \
  collection_object.nq \
  collection_subject.nq \
  double_lower_case_e.nq \
  empty_collection.nq \
  first.nq \
  labeled_blank_node_graph.nq \
  labeled_blank_node_object.nq \
  labeled_blank_node_subject.nq \
  langtagged_LONG_with_subtag.nq \
  langtagged_non_LONG.nq \
  lantag_with_subtag.nq \
  last.nq \
  literal_false.nq \
  literal_true.nq \
  literal_with_BACKSPACE.nq \
  literal_with_CARRIAGE_RETURN.nq \
  literal_with_CHARACTER_TABULATION.nq \
  literal_with_FORM_FEED.nq \
  literal_with_LINE_FEED.nq \
  literal_with_REVERSE_SOLIDUS.nq \
  literal_with_numeric_escape4.nq \
  localName_with_PN_CHARS_BASE_char_boundaries.nq \
  localName_with_assigned_nfc_PN_CHARS_BASE_char_boundaries.nq \
  localName_with_assigned_nfc_bmp_PN_CHARS_BASE_char_boundaries.nq \
  localName_with_leading_digit.nq \
  localName_with_leading_underscore.nq \
  localName_with_nfc_PN_CHARS_BASE_char_boundaries.nq \
  localName_with_non_leading_extras.nq \
  localname_with_COLON.nq \
  negative_numeric.nq \
  nested_blankNodePropertyLists.nq \
  nested_collection.nq \
  numeric_with_leading_0.nq \
  objectList_with_two_objects.nq \
  percent_escaped_localName.nq \
  positive_numeric.nq \
  predicateObjectList_with_two_objectLists.nq \
  prefix_reassigned_and_used.nq \
  repeated_semis_not_at_end.nq \
  reserved_escaped_localName.nq \
  trig-eval-struct-01.nq \
  trig-eval-struct-02.nq \
  trig-subm-01.nq \
  trig-subm-02.nq \
  trig-subm-03.nq \
  trig-subm-04.nq \
  trig-subm-05.nq \
  trig-subm-06.nq \
  trig-subm-07.nq \
  trig-subm-08.nq \
  trig-subm-09.nq \
  trig-subm-10.nq \
  trig-subm-11.nq \
  trig-subm-12.nq \
  trig-subm-13.nq \
  trig-subm-14.nq \
  trig-subm-15.nq \
  trig-subm-16.nq \
  trig-subm-17.nq \
  trig-subm-18.nq \
  trig-subm-19.nq \
  trig-subm-20.nq \
  trig-subm-21.nq \
  trig-subm-22.nq \
  trig-subm-23.nq \
  trig-subm-24.nq \
  trig-subm-25.nq \
  trig-subm-26.nq \
  trig-subm-27.nq \
  two_LITERAL_LONG2s.nq \
  underscore_in_localName.nq

# Used to make N-triples output consistent
BASE_URI=http://www.w3.org/2013/TrigTests/
# for rdf-schema.trig
RDF_NS_URI=http://www.w3.org/1999/02/22-rdf-syntax-ns
# for rdfs-namespace.trig
RDFS_NS_URI=http://www.w3.org/2000/01/rdf-schema

ALL_TEST_FILES= README \
	$(TEST_GOOD_FILES) \
	$(TEST_BAD_FILES) \
	$(TEST_EVAL_FILES) \
	$(TEST_BAD_EVAL_FILES) \
	$(TEST_OUT_FILES)

EXTRA_DIST = $(ALL_TEST_FILES)

RAPPER  = $(top_builddir)/utils/rapper
RDFDIFF = $(top_builddir)/utils/rdfdiff

build-rapper:
	@(cd $(top_builddir)/utils ; $(MAKE) rapper$(EXEEXT))

build-rdfdiff:
	@(cd $(top_builddir)/utils ; $(MAKE) rdfdiff$(EXEEXT))

check-local: check-good-trig check-bad-trig check-eval-trig

if MAINTAINER_MODE
check_good_trig_deps = $(TEST_GOOD_FILES)
endif

check-good-trig: build-rapper $(check_good_trig_deps)
	@set +e; result=0; errors=0; failures=''; \
	$(RECHO) "Testing good Trig syntax passes"; \
	for test in $(TEST_GOOD_FILES); do \
	  name=`basename $$test .trig` ; \
	  baseuri=$(BASE_URI)$$test; \
	  $(RECHO) $(RECHO_N) "Checking $$test $(RECHO_C)"; \
	  $(RAPPER) -q -i trig -o nquads file:$(srcdir)/$$test $$baseuri > $$name.res 2> $$name.err; \
	  status=$$?; \
	  if test $$status != 0 -a $$status != 2 ; then \
	    $(RECHO) "FAILED returned status $$status"; result=1; \
	    $(RECHO) $(RAPPER) -q -i trig -o nquads $(srcdir)/$$test $$baseuri '>' $$name.res; \
	    cat $$name.err; \
	    errors=`expr $$errors + 1`; \
	    failures="$$failures $$test"; \
	  elif test $$status = 2 ; then \
	    $(RECHO) "ok with warnings"; grep Warning $$name.err; \
	  else \
	    $(RECHO) "ok"; \
	  fi; \
	  rm -f $$name.res $$name.err; \
	done; \
	$(RECHO) "Result: $$errors errors: $$failures"; \
	set -e; exit $$result

if MAINTAINER_MODE
check_bad_trig_deps = $(TEST_BAD_FILES) $(TEST_BAD_EVAL_FILES)
endif

check-bad-trig: build-rapper $(check_bad_trig_deps)
	@set +e; result=0; errors=0; failures=''; \
	$(RECHO) "Testing bad Trig fails"; \
	for test in $(TEST_BAD_FILES) $(TEST_BAD_EVAL_FILES) ; do \
	  name=`basename $$test .trig` ; \
	  baseuri=$(BASE_URI)$$test; \
	  $(RECHO) $(RECHO_N) "Checking $$test $(RECHO_C)"; \
	  $(RAPPER) -q -i trig -o nquads file:$(srcdir)/$$test $$baseuri > $$name.res 2> $$name.err; \
	  status=$$?; \
	  if test $$status -eq 1 ; then \
	    $(RECHO) "ok"; \
	  elif test $$status -eq 2 ; then \
	    $(RECHO) "FAILED - parsing succeeded with a warning";  result=1; \
	    $(RECHO) $(RAPPER) -q -i trig -o nquads file:$(srcdir)/$$test $$baseuri '>' $$name.res; \
	    cat $$name.res; grep Warning $$name.err; \
	    errors=`expr $$errors + 1`; \
	    failures="$$failures $$test"; \
	  elif test $$status -eq 0 ; then \
	    $(RECHO) "FAILED - parsing succeeded but should have failed"; result=1; \
	    $(RECHO) $(RAPPER) -q -i trig -o nquads file:$(srcdir)/$$test $$baseuri '>' $$name.res; \
	    cat $$name.res; \
	    errors=`expr $$errors + 1`; \
	    failures="$$failures $$test"; \
	  else \
	    $(RECHO) "FAILED - parsing failed with unknown status $$status"; result=1; \
	    $(RECHO) $(RAPPER) -q -i trig -o nquads file:$(srcdir)/$$test $$baseuri '>' $$name.res; \
	    cat $$name.err; \
	    cat $$name.res; \
	    errors=`expr $$errors + 1`; \
	    failures="$$failures $$test"; \
	  fi; \
	  rm -f $$name.res $$name.err ; \
	done; \
	$(RECHO) "Result: $$errors errors: $$failures"; \
	set -e; exit $$result


if MAINTAINER_MODE
check_eval_trig_deps = $(TEST_EVAL_FILES)
endif

check-eval-trig: build-rapper $(check_eval_trig_deps)
	@set +e; result=0; errors=0; failures=''; \
	$(RECHO) "Testing eval Trig"; \
	for test in $(TEST_EVAL_FILES); do \
	  name=`basename $$test .trig` ; \
	  baseuri=$(BASE_URI)$$test; \
	  $(RECHO) $(RECHO_N) "Checking $$test $(RECHO_C)"; \
	  $(RAPPER) -q -i trig -o nquads $(srcdir)/$$name.nq > $$name.nnq; \
	  $(RAPPER) -q -i trig -o nquads $(srcdir)/$$test $$baseuri > $$name.res 2> $$name.err; \
	  status=$$?; \
	  if test $$status != 0 -a $$status != 2 ; then \
	    $(RECHO) "FAILED returned status $$status"; result=1; \
	    $(RECHO) $(RAPPER) -q -i trig -o nquads $(srcdir)/$$test $$baseuri '>' $$name.res; \
	    cat $$name.err; \
	    errors=`expr $$errors + 1`; \
	    failures="$$failures $$test"; \
	  elif $(RDFCOMPARE) $$name.nnq $$name.res >/dev/null 2>&1; then \
	    if test $$status = 2 ; then \
	      $(RECHO) "ok with warnings"; grep Warning $$name.err; \
	    else \
	      $(RECHO) "ok"; \
	    fi; \
	  else \
	    $(RECHO) "FAILED"; result=1; \
	    $(RECHO) $(RAPPER) -q -i trig -o nquads $(srcdir)/$$test $$baseuri '>' $$name.res; \
	    cat $$name.err; \
	    diff $$name.nnq $$name.res; \
	    errors=`expr $$errors + 1`; \
	    failures="$$failures $$test"; \
	  fi; \
	  rm -f $$name.res $$name.err $$name.nnq; \
	done; \
	$(RECHO) "Result: $$errors errors: $$failures"; \
	set -e; exit $$result
