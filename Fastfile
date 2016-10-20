fastlane_version "1.104.0"

default_platform :ios

platform :ios do

  desc "Validações pré commit do git"
  lane :pre_commit do
    puts ' ---> CS: Iniciando rotina de Integração Contínua'

    puts ' ---> CS: Executando testes unitários'
    scan(scheme: “xxx”)

    puts ' ---> CS: Gerando relatório de Testes'
    slather

  end

  desc "Validações pré push do git"
  lane :pre_push do
    puts ' ---> CS: Iniciando da validação de Integração Contínua'

    puts ' ---> CS: Executando testes unitários'
    scan(scheme: “xxx”)

    # puts ' ---> CS: Buildando projeto em modo calabash'
    # match(
    #   app_identifier: “xxx”,
    #   readonly: true
    # )

    # gym(
    #   workspace: “xxx”,
    #   scheme: “xxx”,
    #   # silent: true,
    #   # clean: true
    # )


    puts ' ---> CS: Synx para organização de diretórios'
    synx

    # puts ' ---> CS: Gerando relatório de Testes'
    # slather

  end

end
