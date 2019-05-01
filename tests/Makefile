scrape:
	@newsroom-scrape \
		--urls data/urls.txt \
		--archive data/test.archive

extract:
	@newsroom-extract \
		--archive data/test.archive \
		--dataset data/test.dataset

run:
	@newsroom-run \
		--system example \
		--dataset data/test.dataset \
		--summaries data/test.summaries

score:
	@newsroom-score \
		--dataset data/test.dataset \
		--summaries data/test.summaries \
		--scores data/test.scores \
		--rouge 1,2,L


tables:
	@newsroom-tables \
		--scores data/test.scores

clean:
	@rm data/test.archive   > /dev/null 2> /dev/null || true
	@rm data/test.dataset   > /dev/null 2> /dev/null || true
	@rm data/test.summaries > /dev/null 2> /dev/null || true
	@rm data/test.scores    > /dev/null 2> /dev/null || true