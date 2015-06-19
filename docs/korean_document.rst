Korean documentation
=====================================================

한글 문서를 작성하는 것도 가능합니다.

한글 문서를 작성하기 위한 환경설정
______________________________________________________

- ``conf.py`` 파일을 엽니다.
- ``source_encoding`` 옵션을 찾아 cp949 로 바꾸어 줍니다. ``source_encoding = 'cp949'``
- 이제 한글 문서를 작성할 수 있습니다.

Autodoc 작성을 위한 파이썬 파일에서의 환경설정
________________________________________________________

- 한글로 주석을 남기고 싶은 파이썬 파일 상단에 ``#-*- coding: utf-8 -*-`` 를 추가합니다.
- 다음과 같이 자유롭게 한글로 주석을 남길 수 있습니다.

.. code-block:: python

    #-*- coding: utf-8 -*-

    """
    vmlModuleB 입니다.
    이제 세미나가 거의 끝나갑니다.
    """

    def vmlModule_fuctionC(argA, argB) :
        """
        이 함수는 vmlModule_functionC 함수입니다.
        2개의 파라미터(argA, argB) 를 받아서, argA 에서 argB 를 뺀 결과를 반환하는 함수입니다.

        :param argA: argumentA 입니다.
        :param argB: argumentB 입니다.
        :return: argA-argB. 결과를 반환합니다.
        """
        return argA - argB

- 문서 결과물은 다음 링크에서 볼 수 있습니다.
- :ref:`vmlModuleB-label`

